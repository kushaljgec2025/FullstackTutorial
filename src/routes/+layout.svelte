<script>
import Navbar from "../components/Navbar.svelte";
import Footer from "../components/Footer.svelte";
import "../app.css";
</script>


<Navbar/>
<div class="min-h-[70vh] flex flex-col justify-center items-center">
    <slot/>
</div>
<Footer/>