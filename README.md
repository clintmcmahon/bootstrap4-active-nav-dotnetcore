# Bootstrap 4 Active Nav
Simple way to place the "active" class into the current nav item in Bootstrap 4 using .Net MVC

```

<nav class="navbar navbar-expand-md bg-light navbar-light">
        <div class="container">
            <div class="navbar-collapse collapse pt-2 pt-md-0" id="navbar2">
                <ul class="navbar-nav mr-auto">
                    <li class='nav-item @(Context.Request.Path == "/" ? "active" : "")'>
                        <a class="nav-link" href="/">Home</a>
                    </li>
                    <li class='nav-item @(Context.Request.Path == "/path1" ? "active" : "")'>
                        <a class="nav-link" href="/path1">Path 1</a>
                    </li>
                    <li class='nav-item @(Context.Request.Path == "/path2" ? "active" : "")'>
                        <a class="nav-link" href="/path2">Path 2</a>
                    </li>
                    <li class='nav-item @(Context.Request.Path == "/path3" ? "active" : "")'>
                        <a class="nav-link" href="/path3">Path 3</a>
                    </li>
                </ul>
            </div>
        </div>
</nav>
```
