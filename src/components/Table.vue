<template>
    <div>
        <table class="table has-text-centered">
            <thead>
                <tr>
                <th><abbr title="Nomor">No</abbr></th>
                <th><abbr title="Mata Kuliah">Matkul</abbr></th>
                <th>Jadwal</th>
                <th>Timer</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="(jadwal, index) in jadwals" :key="index">
                    <th>{{index + 1}}</th>
                    <td>{{jadwal.matkul}}</td>
                    <td>{{jadwal.tanggal}}</td>
                    <td><Timer v-bind:date="jadwal.date"></Timer></td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
import Timer from './Timer'
export default {
    components: {
        Timer
    },
    data(){
        return{
            jadwals: [
                {
                    matkul: 'Basis Data',
                    tanggal: '9 Desember 2019',
                    date: 'December 09, 2019'
                },
                {
                    matkul: 'Sistem Operasi',
                    tanggal: '11 Desember 2019',
                    date: 'December 11, 2019'
                },
                {
                    matkul: 'Studium Generale',
                    tanggal: '13 Desember 2019',
                    date: 'December 13, 2019'
                },
                {
                    matkul: 'Jaringan dan Komunikasi Data',
                    tanggal: '16 Desember 2019',
                    date: 'December 16, 2019'
                },
                {
                    matkul: 'Matematika Diskret dan Logika',
                    tanggal: '17 Desember 2019',
                    date: 'December 17, 2019'
                },
                {
                    matkul: 'Isyarat dan Sistem (Kuliah+Tutorial)',
                    tanggal: '18 Desember 2019',
                    date: 'December 18, 2019'
                },
                {
                    matkul: 'Sistem Mikroprosesor',
                    tanggal: '19 Desember 2019',
                    date: 'December 19, 2019'
                },
                {
                    matkul: 'Teknik Pemodelan dan Simulasi',
                    tanggal: '20 Desember 2019',
                    date: 'December 20, 2019'
                },
            ]
        }
    }
}
</script>