<template>
    <div>
        <Sidebar />
        <div class="right-panel" id="right-panel">
            <Header />

            <!-- Content -->
            <div class="content">
                <div class="animated fadeIn">
                    <div class="row">
                        <div class="col-lg-12">
                            <div class="card">
                                <div class="card-header">
                                    <strong class="card-title">Data Seluruh Kader</strong>
                                </div>
                                <div class="table-stats order-table ov-h">
                                    <table class="table ">
                                        <thead>
                                            <tr>
                                                <th class="serial">#</th>
                                                <th class="avatar">Avatar</th>
                                                <th>ID</th>
                                                <th>Nama Lengkap</th>
                                                <th>Nim</th>
                                                <th>Prodi</th>
                                                <th>Jenis Kelamin</th>
                                                <th>Tanggal Lahir</th>
                                                <th>Tempat Lahir</th>
                                                <th>No. HP</th>
                                                <th>Asal</th>
                                                <th>Generation</th>
                                            </tr>
                                        </thead>
                                        <tbody>
                                            <tr v-for="data in kader" :key="data.id">
                                                <td class="serial">1.</td>
                                                <td class="avatar">
                                                    <div class="round-img">
                                                        <a href="#"><img class="rounded-circle" src="images/avatar/1.jpg" alt=""></a>
                                                    </div>
                                                </td>
                                                <td> #{{ data.id }} </td>
                                                <td> <span class="name">{{ data.nama_lengkap }}</span> </td>
                                                <td> <span class="product">{{ data.nim }}</span> </td>
                                                <td><span class="count">{{ data.prodi }}</span></td>
                                                <td>
                                                    <span class="badge badge-complete">{{ data.jenis_kelamin }}</span>
                                                </td>
                                                <td>{{ data.tanggal_lahir }}</td>
                                                <td>{{ data.tempat_lahir }}</td>
                                                <td>{{ data.no_hp }}</td>
                                                <td>{{ data.asal }}</td>
                                                <td>{{ data.generation }}</td>
                                            </tr>
                                        </tbody>
                                    </table>
                                </div>
                                <!-- /.table-stats -->
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <!-- /.content -->
            <!-- <div class="clearfix"></div> -->
        </div>
    </div>
</template>

<script>
import Sidebar from '../../../components/admin/Sidebar.vue';
import Header from '../../../components/admin/Header.vue';
import axios from 'axios';

export default {
    name: 'Kader',
    components: {
        Sidebar,
        Header,
    },
    data() {
        return {
            kader: null
        }
    },
    mounted() {
        axios.get(`https://apimaroon.zainportfolio.com/kader`).then(response => {
            this.kader = response.data
            return this.kader
        })
    }

}
</script>