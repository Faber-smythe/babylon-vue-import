<script lang="ts">
import * as BABYLON from 'babylonjs'
import 'babylonjs-loaders'

export default {
  props:{
    msg: String
  },
  async mounted(){
    /**
     * SETUP
     */
    const canvas = this.$refs.renderCanvas as HTMLCanvasElement
    const engine = new BABYLON.Engine(canvas)
    const scene = new BABYLON.Scene(engine)
    const camera = new BABYLON.ArcRotateCamera('myCamera', 1.56, 1.56, 5, new BABYLON.Vector3(0, 0.5, 0), scene)
    camera.attachControl(canvas)
    scene.createDefaultEnvironment()

    /**
     * IMPORT MESH HERE
     */
    await BABYLON.SceneLoader.ImportMeshAsync("",
      "",
      "y-bot.glb",
      scene);


    /**
     * RENDER SCENE
     */
    engine.runRenderLoop(()=>{
      scene.render()
    })
  }
}
</script>

<template>
  <canvas id="renderCanvas" ref="renderCanvas"></canvas>
  <h2><a target="_blank" href="https://www.mixamo.com/">{{ msg }}</a></h2>
</template>

<style scoped>
#renderCanvas{
  border: 1px solid red;
  height: 500px;
  width: 850px;
}
</style>
