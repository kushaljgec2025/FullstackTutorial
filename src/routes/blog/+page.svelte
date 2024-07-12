<script>
    let name=""
    let slug=name
    export function handelChange(event){
       slug = event.target.value.replace(/\s+/g, '-');
    }
</script>


<h1 class="text-red-500 text-3xl font-bold">
    Welcome to Blog
</h1>
<p>Write you blog title</p>
<form  action={`blog/${slug}`}>
    <input type="text" class="bg-gray-300 px-4 py-2 outline-none rounded-full" bind:value={name} on:input={handelChange}>
    <button type="submit" class="bg-gray-300 p-2">Submit</button>

</form>
<span class="text-black">
    Slug :{slug}
</span>

