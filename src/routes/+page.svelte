<script>
    import '../lib/internal/main.js';
    var term;
    var winwidth;
    var winheight;
    var evol = new Evol(winheight,winwidth);
    evol.start(term);
    import { io } from "socket.io-client";
    import Evol from '../lib/internal/main.js';
</script>

<svelte:window bind:innerHeight={winheight} bind:innerWidth={winwidth}></svelte:window>
<pre class="terminalscreen" id="term" bind:this={term}>
    
</pre>