<script setup>
import SideBar from '../components/Dashboard/SideBar.vue'
// import Chart from '../components/Dashboard/Chart.vue'

</script>


<template>
    <main class="bg-zinc-950 h-screen">
        <div class="w-full">
            <div class="grid grid-cols-5 w-full">
                <div class="col-span-1 ">
                    <SideBar />
                </div>
                <div class="col-span-4">
                    <div class="content p-12 h-screen w-full text-white space-y-14">
                        <div class="title">
                            <h1 class=" text-white text-2xl font-bold  text-left">Manage Your Market</h1>
                            <p class="text-gray-400">Track your market graph here</p>
                        </div>
                        <div class="dashboard-information">
                            <div class="grid grid-cols-7">
                                <div class="col-span-2 bg-zinc-900 rounded-lg m-1 p-4">
                                    <h2 class="text-l font-bold">PENJUALAN</h2>
                                    <!-- <Chart /> -->
                                </div>
                                <div class="col-span-3 bg-zinc-900 rounded-lg m-1 p-4">
                                    <h2 class="text-m font-bold">STOCK</h2>    
                                </div>
                                <div class="col-span-2 bg-zinc-900 rounded-lg m-1 p-4">
                                    <h2 class="text-m font-bold">PENDAPATAN</h2>
                                </div>
                            </div>
                        </div>
                        <div class="transaction-activity space-y-12">
                            <h2 class="font-bold">Transaction Activity</h2>
                            <div class="table-transaction">
                                <table class="table-auto w-full">
                                <thead>
                                    <tr>
                                    <th class="text-left text-zinc-500">User</th>
                                    <th class="text-left text-zinc-500">Tanggal</th>
                                    <th class="text-left text-zinc-500">Jumlah Product</th>
                                    <th class="text-left text-zinc-500">Pembelian</th>
                                    </tr>
                                </thead>
                                <tbody>
                                    <tr>
                                    <td>Unknown</td>
                                    <td>Malcolm Lockyer</td>
                                    <td>1961</td>
                                    <td>1961</td>
                                    </tr>
                                    <tr>
                                    <td>Unknown</td>
                                    <td>The Eagles</td>
                                    <td>1961</td>
                                    <td>1972</td>
                                    </tr>
                                    <tr>
                                    <td>Unknown</td>
                                    <td>Earth, Wind, and Fire</td>
                                    <td>1961</td>
                                    <td>1975</td>
                                    </tr>
                                </tbody>
                                </table>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<style>
    main{
        font-family: 'Montserrat', sans-serif;
    }
</style>