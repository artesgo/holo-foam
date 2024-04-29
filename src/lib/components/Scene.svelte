<script lang="ts">
  import { T } from '@threlte/core'
  import { ContactShadows, Float, Grid } from '@threlte/extras'
  import { Bae, Fauna, IRyS, Kronii, Mumei, Sana } from './models';
	import Player from '$lib/player/player.svelte';
</script>

<T.DirectionalLight
  intensity={0.8}
  position.x={5}
  position.y={10}
/>

<T.AmbientLight intensity={0.2} />

<Grid
  position.y={-0.001}
  cellColor="#ffffff"
  sectionColor="#ffffff"
  sectionThickness={0}
  fadeDistance={25}
  cellSize={2}
/>

<ContactShadows
  scale={10}
  blur={2}
  far={2.5}
  opacity={0.5}
/>

<Float
  floatIntensity={1}
  floatingRange={[0, 0.1]}
>
  <T.Mesh
    position.y={0}
    position.x={1.25}
    position.z={-2}
    scale={3}
  >
    <Sana />
    <T.MeshStandardMaterial color="#F85122" />
  </T.Mesh>
</Float>

<Float
  floatIntensity={1}
  floatingRange={[0, 0.1]}
>
  <T.Mesh
    position.y={0}
    position.x={-1}
    position.z={-0.75}
  >
    <Bae />
    <T.MeshStandardMaterial color="#F85122" />
  </T.Mesh>
</Float>

<Float
  floatIntensity={1}
  floatingRange={[0, 0.1]}
>
  <T.Mesh
    position.y={0}
    position.z={-0.75}
  >
    <IRyS />
    <T.MeshStandardMaterial color="#F85122" />
  </T.Mesh>
</Float>

<Float
  floatIntensity={1}
  floatingRange={[0, 0.1]}
>
  <T.Mesh
    position.y={0}
    position.x={1}
    position.z={-0.75}
  >
    <Mumei />
    <T.MeshStandardMaterial color="#F85122" />
  </T.Mesh>
</Float>

<Float
  floatIntensity={1}
  floatingRange={[0, 0.1]}
>
  <T.Mesh
    position.y={0}
    position.x={2}
    position.z={-0.75}
  >
    <Fauna />
    <T.MeshStandardMaterial color="#F85122" />
  </T.Mesh>
</Float>

<Float
  floatIntensity={1}
  floatingRange={[0, 0.1]}
>
  <T.Mesh
    position.y={0}
    position.x={3}
    position.z={-0.75}
  >
    <Kronii />
    <T.MeshStandardMaterial color="#F85122" />
  </T.Mesh>
</Float>

<Player />

<!-- 
<Float
  floatIntensity={1}
  floatingRange={[0, 1]}
>
  <T.Mesh
    position={[1.2, 1.5, 0.75]}
    rotation.x={5}
    rotation.y={71}
  >
    <T.TorusKnotGeometry args={[0.5, 0.15, 100, 12, 2, 3]} />
    <T.MeshStandardMaterial color="#F85122" />
  </T.Mesh>
</Float>

<Float
  floatIntensity={1}
  floatingRange={[0, 1]}
>
  <T.Mesh
    position={[-1.4, 1.5, 0.75]}
    rotation={[-5, 128, 10]}
  >
    <T.IcosahedronGeometry />
    <T.MeshStandardMaterial color="#F8EBCE" />
  </T.Mesh>
</Float> -->
