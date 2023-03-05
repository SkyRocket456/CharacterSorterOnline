<script>
    import {Router, Route, Link} from "svelte-routing";
    import Home from "./routes/Home.svelte";
    import Blog from "./routes/Sort.svelte";

    export let url = "";
</script>

<Router url="{url}">
    <nav>
        <Link to="/">Home</Link>
        <Link to="blog">Blog</Link>
    </nav>
    <div>
        <Route path="/"><Home/>
        </Route>
        <Route path="blog" component="{Blog}"/>
    </div>
</Router>