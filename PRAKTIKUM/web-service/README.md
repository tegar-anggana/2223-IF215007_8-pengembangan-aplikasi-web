```javascript
const express = require('express')
const app = express()
const port = 3000
const cors = require('cors')

app.use(cors({
  origin: '*'
}));

// app.get('/', (req, res) => {
//   res.send('Hello world!')
// })

// Lihat list halaman
app.get('/halaman', (req, res) => {
  res.json([
    {
      nama: 'Tugas Kuliah',
      pembuat: 'Tegar'
    },
    {
      nama: 'Tugas Customer Service',
      pembuat: 'Levta'
    }
  ])
})

// Lihat detail halaman
app.get('/halaman/:id', (req, res) => {
  res.json(
    {
      nama: 'Tugas Kuliah',
      pembuat: 'Tegar'
    },
  )
})

// Tambah halaman
app.post('/halaman', (req, res) => {
  res.json(
    {
      id: 3,
      nama: "HIMATIF",
      pembuat: "Gargar"
    }
  )
})


app.listen(port, () => {
  console.log(`Example app listening on port ${port}`)
})
```
