# data-barang
tugas data barang bu nisa menggunakan html dengan format php
<!doctype html>
<html lang="en">
  <head>
    <!-- Required meta tags -->
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">

    <!-- Bootstrap CSS -->
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">

    <title>CRUD PHP MySQL Bootstrap</title>
  </head>
  <body>
    
  <nav class="navbar navbar-light bg-light">
  <div class="container-fluid">
    <form class="d-flex">
      <input class="form-control me-2" type="search" placeholder="Search" aria-label="Search">
      <button class="btn btn-outline-success" type="submit">Search</button>
    </form>
  </div>
</nav>
<form method="GET" class="mb-3">
    <select name="filter" class="form-select" onchange="this.form.submit()">
        <option value="" disabled selected>Pilih Kategori</option>
        <option value="harga_asc">Harga Terendah</option>
        <option value="harga_desc">Harga Tertinggi</option>
        <option value="stok_habis">Stok Habis</option>
    </select>
</form>
<button type="button" class="btn btn-primary" data-bs-toggle="modal" data-bs-target="#addModal">Tambah Barang</button>

<div class="modal fade" id="addModal" tabindex="-1">
    <div class="modal-dialog">
        <div class="modal-content">
            <div class="modal-header">
                <h5 class="modal-title">Tambah Barang</h5>
                <button type="button" class="btn-close" data-bs-dismiss="modal"></button>
            </div>
            <div class="modal-body">
                <form>
                    <div class="mb-3">
                        <label for="nama" class="form-label">Nama Barang</label>
                        <input type="text" class="form-control" id="nama" required>
                    </div>
                    <div class="mb-3">
                        <label for="harga" class="form-label">Harga</label>
                        <input type="number" class="form-control" id="harga" required>
                    </div>
                    <button type="submit" class="btn btn-success">Simpan</button>
                </form>
            </div>
        </div>
    </div>
</div>

<div class="container mt-5">
    <h1>Data Barang</h1>
    <table class="table  table-bordered table-striped">
        <thead>
            <tr>
                <th>No</th>
                <th>Nama</th>
                <th>Jumlah</th>
                <th>Harga</th>
                <th>Tanggal</th>
                <th>Aksi</th>
                <th>Detail</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>1.</td>
                <td>iPhone XR RAM 64GB</td>
                <td>23</td>
                <td>4.890.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
                <td>2.</td>
                <td>iPhone XR RAM 128GB</td>
                <td>41</td>
                <td>5.490.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
            </td>
            </tr>
            <tr>
                <td>3.</td>
                <td>iPhone XR RAM 256GB</td>
                <td>28</td>
                <td>5.950.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
                <td>4.</td>
                <td>iPhone 11 RAM 64GB</td>
                <td>13</td>
                <td>6.249.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>5.</td>
                <td>iPhone 11 RAM 128GB</td>
                <td>44</td>
                <td>7.749.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>6.</td>
                <td>iPhone 12 RAM 64GB</td>
                <td>50</td>
                <td>8.249.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>7.</td>
                <td>iPhone 12 RAM 128GB</td>
                <td>90</td>
                <td>9.249.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>8.</td>
                <td>iPhone 12 RAM 256GB</td>
                <td>67</td>
                <td>9.249.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>9.</td>
                <td>iPhone 13 RAM 128GB</td>
                <td>30</td>
                <td>10.249.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>10.</td>
                <td>iPhone 13 RAM 256GB</td>
                <td>50</td>
                <td>12.749.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>11.</td>
                <td>iPhone 13 RAM 512GB</td>
                <td>40</td>
                <td>12.749.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>12.</td>
                <td>iPhone 14 RAM 128GB</td>
                <td>50</td>
                <td>12.249.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>13.</td>
                <td>iPhone 14 RAM 256GB</td>
                <td>55</td>
                <td>15.049.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>

                </td>
            </tr>
            <tr>
            <tr>
                <td>14.</td>
                <td>iPhone 14 RAM 512GB</td>
                <td>10</td>
                <td>15.999.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>15.</td>
                <td>iPhone 14 Plus RAM 128GB</td>
                <td>5</td>
                <td>12.499.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>16.</td>
                <td>iPhone 14 Plus RAM 256GB</td>
                <td>7</td>
                <td>14.999.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>17.</td>
                <td>iPhone 14 Plus RAM 512GB</td>
                <td>13</td>
                <td>17.999.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
                <td>18.</td>
                <td>iPhone 14 Pro RAM 128GB</td>
                <td>10</td>
                <td>16.999.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
            <tr>
                <td>19.</td>
                <td>iPhone 14 Pro RAM 256GB</td>
                <td>25</td>
                <td>14.499.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
            <tr>
                <td>20.</td>
                <td>iPhone 14 Pro RAM 512GB</td>
                <td>25</td>
                <td>20.999.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
            <tr>
                <td>21.</td>
                <td>iPhone 14 Pro RAM 1TB</td>
                <td>10</td>
                <td>24.890.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <tr>
            <tr>
                <td>22.</td>
                <td>iPhone 14 Pro Max RAM 128GB</td>
                <td>5</td>
                <td>15.999.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            
            <tr>
                <td>23.</td>
                <td>iPhone 15 RAM 128GB</td>
                <td>50</td>
                <td>14.249.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td>
            </tr>
            <tr>
            <td>24.</td>
                <td>iPhone 15 RAM 256GB</td>
                <td>57</td>
                <td>17.249.000</td>
                <td>13/01/2025</td>
                <td width="15%" class="text-center">
                <button type="button" class="btn btn-success">Edit</button>
                <button type="button" class="btn btn-danger">Hapus</button>
                <td>
                <button class="btn btn-info" data-bs-toggle="modal" data-bs-target="#modalDetail1">Detail</button>
                </td>
                </td> 
        </tbody>
</table>
</div>
<canvas id="myChart" width="400" height="200"></canvas>
<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script>
    const ctx = document.getElementById('myChart').getContext('2d');
    const myChart = new Chart(ctx, {
        type: 'bar',
        data: {
            labels: ['iPhone XR', 'iPhone 11', 'iPhone 12', 'iPhone 13', 'iPhone 14', 'iPhone 15'],
            datasets: [{
                label: 'Jumlah Barang',
                data: [92, 53, 251, 120, 210, 107],
                backgroundColor: ['#872341', '#E7D283', '#16C47F', '#B7E0FF', '#B771E5', '#C890A7']
            }]
        }
    });
</script>


    <!-- Optional JavaScript; choose one of the two! -->

    <!-- Option 1: Bootstrap Bundle with Popper -->
    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>

   
  </body>
</html>
