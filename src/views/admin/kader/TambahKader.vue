<template>
    <div>
        <Sidebar />
        <div class="right-panel" id="right-panel">
            <Header />

            <!-- Content -->
            <div class="content">
                <!-- Animated -->
                <div class="animated fadeIn">
                    <!-- Widgets  -->
                    <div class="row">
                        <div class="col-lg-6 col-md-6">
                            <div class="card">
                                <div class="card-body">
                                    <div class="stat-widget-five">
                                        <div class="stat-icon dib flat-color-1">
                                            <i class="pe-7s-cash"></i>
                                        </div>
                                        <div class="stat-content">
                                            <div class="text-left dib">
                                                <div class="stat-text">Rp. <span class="count">123901212</span></div>
                                                <div class="stat-heading">Penghasilan</div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <div class="col-lg-6 col-md-6">
                            <div class="card">
                                <div class="card-body">
                                    <div class="stat-widget-five">
                                        <div class="stat-icon dib flat-color-2">
                                            <i class="pe-7s-cart"></i>
                                        </div>
                                        <div class="stat-content">
                                            <div class="text-left dib">
                                                <div class="stat-text"><span class="count">3435</span></div>
                                                <div class="stat-heading">Penjualan</div>
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <!-- /Widgets -->
                <!-- /#add-category -->
                </div>
                <!-- .animated -->
            </div>
            <!-- /.content -->
            <!-- <div class="clearfix"></div> -->
        </div>
    </div>
</template>

<script>
import Sidebar from '../../../components/admin/Sidebar.vue';
import Header from '../../../components/admin/Header.vue';

export default {
    name: 'TambahKader',
    components: {
        Sidebar,
        Header,
    }

}
</script>