<template>
    <div>
        <table class="table">
        <thead>
            <tr>
            <th scope="col">Title</th>
            <th scope="col">Artist</th>
            <th scope="col">Genre</th>
            <th scope="col">Album</th>
            </tr>
        </thead>
        <tbody v-for="(song, index) in songs" v-bind:key="index">
            <tr>
            <td>{{song.title}}</td>
            <td>{{song.artist}}</td>
            <td>{{song.genre}}</td>
            <td>{{song.album}}</td>
            </tr>
        </tbody>
        </table>
    </div>
</template>

<script>

import MusicData from '../assets/list.json'

export default {
    data() {
        return {
            songs: MusicData
        }
    }
}
</script>

<style>
    
</style>