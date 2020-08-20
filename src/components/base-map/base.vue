<template>
    <vl-map style="height: 90vh" data-projection="EPSG:4326">
        <vl-view :zoom.sync="zoom" :center.sync="center"></vl-view>
        <vl-layer-tile :z-index="0">
            <vl-source-osm></vl-source-osm>
        </vl-layer-tile>


    </vl-map>
</template>

<script>
    export default {
        data() {
            return {
                zoom: 14,
                center: [28.810868035076453, 41.09428681546953],
                rotation: 0,
            }
        }
    }
</script>