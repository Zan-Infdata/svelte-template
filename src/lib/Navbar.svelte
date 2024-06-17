<script lang="ts">

export let active: number = 0;

</script>

<!-- Navigation-->
<nav class="navbar navbar-expand-lg navbar-light bg-light">
    <div class="container px-4 px-lg-5">
        <a class="navbar-brand" href="#!">JerryTable</a>
        <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation"><span class="navbar-toggler-icon"></span></button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
            <ul class="navbar-nav me-auto mb-2 mb-lg-0 ms-lg-4">
                <li class="nav-item"><a class="nav-link" class:active={active == 0} href="/">Tables</a></li>
                <li class="nav-item"><a class="nav-link" class:active={active == 1} href="#/orders">Orders</a></li>
                <li class="nav-item dropdown">
                    <a class="nav-link dropdown-toggle" class:active={active == 2} id="navbarDropdown" href="#" role="button" data-bs-toggle="dropdown" aria-expanded="false">Add</a>
                    <ul class="dropdown-menu" aria-labelledby="navbarDropdown">
                        <li><a class="dropdown-item" href="#/table/add">Table</a></li>
                        <li><hr class="dropdown-divider" /></li>
                        <li><a class="dropdown-item" href="#/drink/add">Drink</a></li>
                    </ul>
                </li>
            </ul>
        </div>
    </div>
</nav>