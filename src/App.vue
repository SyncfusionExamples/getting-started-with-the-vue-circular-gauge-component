<script setup>
import { CircularGaugeComponent as EjsCirculargauge, AxesDirective as EAxes,
         AxisDirective as EAxis, PointersDirective as EPointers,
         PointerDirective as EPointer, RangesDirective as ERanges,
         RangeDirective as ERange
 } from '@syncfusion/ej2-vue-circulargauge';
 const cap = 
 {
    radius : 20
 }
 const labelStyle=
 {
    position: 'Outside'
 }
</script>

<template>
<ejs-circulargauge>
    <e-axes>
        <e-axis startAngle="270" endAngle="90" radius="150" :labelStyle="labelStyle">
            <e-pointers>
                <e-pointer value="40" :cap="cap"></e-pointer>
            </e-pointers>
            <e-ranges>
                <e-range start="40" end="100"></e-range>
            </e-ranges>
        </e-axis>
    </e-axes>
</ejs-circulargauge>
</template>

<style scoped>

</style>
