<script lang="ts">
    export let elementIndex: number;
</script>

<div class="hex-tile">
    <span>{elementIndex}</span>
</div>

<style>
 .hex-tile {
  width: 51px;
  height: 28px;
  background: red;
  position: absolute;
}
.hex-tile:before {
  content: "";
  position: absolute;
  top: -13px;
  left: 0;
  width: 0;
  height: 0;
  border-left: 25px solid transparent;
  border-right: 25px solid transparent;
  border-bottom: 13px solid red;
}
.hex-tile:after {
  content: "";
  position: absolute;
  bottom: -13px;
  left: 0;
  width: 0;
  height: 0;
  border-left: 25px solid transparent;
  border-right: 25px solid transparent;
  border-top: 13px solid red;
}
</style>