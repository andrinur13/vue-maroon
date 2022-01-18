<template>
    <div class="text-left">
        <!-- Left Panel -->
        <aside id="left-panel" class="left-panel">
            <nav class="navbar navbar-expand-sm navbar-default">
                <div id="main-menu" class="main-menu collapse navbar-collapse">
                    <ul class="nav navbar-nav">
                        
                        <router-link tag="li" to="/dashboard">
                            <a><i class="menu-icon fa fa-laptop"></i>Dashboard </a>
                        </router-link>
                        
                        <li class="menu-title">Barang</li><!-- /.menu-title -->
    
                        <router-link tag="li" to="/kader"> 
                            <a><i class="menu-icon fa fa-list"></i>Data Kader</a>
                        </router-link>
                        
                        <router-link tag="li" to="/tambah-kader"> 
                            <a><i class="menu-icon fa fa-plus"></i>Tambah Kader</a>
                        </router-link>

                        <li class="menu-title">Foto Barang</li><!-- /.menu-title -->
                        <li class="">
                            <router-link to="#"> <i class="menu-icon fa fa-list"></i>Lihat Foto Barang</router-link>
                        </li>
                        <li class="">
                            <a href="#"> <i class="menu-icon fa fa-plus"></i>Tambah Foto Barang</a>
                        </li>

                        <li class="menu-title">Transaksi</li><!-- /.menu-title -->
                        <li class="">
                            <router-link to="#"> <i class="menu-icon fa fa-list"></i>Lihat Transaksi</router-link>
                        </li>
                    </ul>
                </div><!-- /.navbar-collapse -->
            </nav>
        </aside>
        <!-- /#left-panel -->
    </div>
</template>

<script>
import 'jquery'
import '../../assets/assets/js/main.js';

export default {
    name: 'Sidebar',
    
    mounted(){
        // this.sidebar()
    },
    methods: {
        // sidebar(){
        //     const menuToggle = document.querySelector('#menuToggle');
        //     menuToggle.addEventListener("click", function(){ 
        //         var windowsWidth = window.document.innerWidth;
        //         if(windowsWidth < 1010){
        //             const body = document.querySelector('body');
        //             body.classList.remove('open')
        //             const lf_panel = document.querySelector('#left-panel')
        //             if (windowsWidth<760){
        //                 lf_panel.style.display = "block"
        //             } else {
        //                 lf_panel.classList.toggle('open-menu')
        //             } 
        //         }else{
        //             const body = document.querySelector('body');
        //             body.classList.toggle('open')
        //         }
        //     })
        // },
    }
}
</script>