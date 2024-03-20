<script>
  import {Router, Route, Link} from 'svelte-routing'
  import Contact from './components/Contact.svelte';
  import Home from './components/Home.svelte';
  import About from './components/About.svelte';

</script>
<Router>
  <nav class="flex justify-between shadow p-4">
    <div><a href="/"><span class=" font-bold text-lg text-slate-800" style="">andr3ick</span></a></div>
    <div class="space-x-6">
     <Link to="/">Home</Link> 
     <Link to="/about">About Me</Link> 
     <Link to="/contact">Contact</Link> 
    </div>
    <div></div>
    </nav>

  <Route path="/">
   <Home/>
  </Route>

  <Route path="/about">
    <About/>
    </Route>

    <Route path="/contact">
      <Contact/>
      </Route>

    <footer class="text-center p-3">
      <div class="border-t-2 border-gray-200 mx-[20%] mb-5"></div>
      <h3 class="text-2xl mb-5">Follow me</h3>
      <div class="p-4 space-x-6">
        <a href="https://github.com/kundaiO6" class="bg-gray-100 text-gray-500 p-3 rounded-lg text-2xl hover:text-slate-800"><span class="bi bi-github"></span></a>
        <a href="https://www.linkedin.com/in/kundai-chifwafwa-091b75262" class="bg-gray-100 text-gray-500 p-3 rounded-lg text-2xl hover:text-slate-800" ><span class="bi bi-linkedin"></span></a>
        <a href="https://twitter.com/Kundai061" class="bg-gray-100 text-gray-500 p-3 rounded-lg text-2xl hover:text-slate-800" ><span class="bi bi-twitter"></span></a>
        <a href="https://medium.com/@kundaichifwafwa" class="bg-gray-100 text-gray-500 p-3 rounded-lg text-2xl hover:text-slate-800" ><span class="bi bi-medium"></span></a>
      </div>
    </footer>
</Router>