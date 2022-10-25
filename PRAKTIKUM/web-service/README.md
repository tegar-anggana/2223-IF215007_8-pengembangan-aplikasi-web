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
    }
  )
})

// Lihat list tugas
app.get('/halaman/:id/tugas', (req, res) => {
  res.json([
    {
      id: 1,
      nama: 'Membuat aplikasi web berbasis React',
      halaman: 'Tugas Kuliah',
      deadline: '1 Juli 2020',
      status_selesai: 'Belum',
      subtasks: [
        {
          nama: 'Merancang frontend',
          deadline: '2 Juli 2022',
          status_selesai: 'Sudah',
          task: 'Membuat aplikasi web berbasis React'
        },
        {
          nama: 'Merancang frontend',
          deadline: '2 Juli 2022',
          status_selesai: 'Sudah',
          task: 'Membuat aplikasi web berbasis React'
        }
      ],
      properti_kustom: [
        {
          nama: 'Mata Kuliah',
          value: 'Manajemen Basis Data'
        },
        {
          nama: 'Kesulitan',
          value: 'Sulit Banget'
        },
        {
          nama: 'Individu / Kelompok',
          value: 'Individu'
        }
      ]
    },
    {
      id: 2,
      nama: 'Membuat resume tentang ImageJ',
      halaman: 'Tugas Kuliah',
      deadline: '1 Maret 2023',
      status_selesai: 'Belum',
      subtasks: [],
      properti_kustom: [
        {
          nama: 'Mata Kuliah',
          value: 'Artificial Intelligence'
        },
        {
          nama: 'Kesulitan',
          value: 'Sangat Mudah'
        },
        {
          nama: 'Individu / Kelompok',
          value: 'Kelompok'
        }
      ]
    }
  ])
})

// Lihat detail tugas
app.get('/halaman/:id/tugas/:id', (req, res) => {
  res.json(
    {
      id: 1,
      nama: 'Membuat aplikasi web berbasis React',
      halaman: 'Tugas Kuliah',
      deadline: '1 Juli 2020',
      status_selesai: 'Belum',
      subtasks: [
        {
          nama: 'Merancang frontend',
          deadline: '2 Juli 2022',
          status_selesai: 'Sudah',
          task: 'Membuat aplikasi web berbasis React'
        },
        {
          nama: 'Merancang frontend',
          deadline: '2 Juli 2022',
          status_selesai: 'Sudah',
          task: 'Membuat aplikasi web berbasis React'
        }
      ],
      properti_kustom: [
        {
          nama: 'Mata Kuliah',
          value: 'Manajemen Basis Data'
        },
        {
          nama: 'Kesulitan',
          value: 'Sulit Banget'
        },
        {
          nama: 'Individu / Kelompok',
          value: 'Individu'
        }
      ]
    }
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
