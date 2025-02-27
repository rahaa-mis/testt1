<template>
<div class="d-flex bg-light">
    <aside id="sidebar">
        <div class="sidebar-logo">
            <div class="logo-header">
                <img src="@/assets/LOGO.png" alt="Company Logo" class="logo" />
                <h2 class="team-text">HI TEAM</h2>
            </div>
        </div>

        <ul class="sidebar-nav p-1">
            <li class="sidebar-item" id="dashboard" style="background-color: #6366F1">
                <a href="#" class="sidebar-link" style="color:white;">
                    <i class="bi bi-house-door"></i>
                    <span> Dashboard</span>
                </a>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-box-seam"></i>
                    <span> Orders</span>
                </a>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-people"></i>
                    <span> Passengers</span>
                </a>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-car-front"></i>
                    <span> Captains</span>
                </a>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-clipboard-minus"></i>
                    <span> Categories</span>
                </a>
                <hr>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-file-text"></i>
                    <span> Settlement</span>
                </a>
                <hr>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-chat-dots"></i>
                    <span> Contact</span>
                </a>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-stars"></i>
                    <span> Reviews</span>
                </a>
                <hr>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link collapsed has-dropdown" data-bs-toggle="collapse" data-bs-target="#dropmenu" aria-expanded="true" aria-controls="dropmenu">
                    <i class="bi bi-shield-lock"></i>
                    <span> Permissions</span>
                </a>
                <ul id="dropmenu" class="sidebar-dropdown list-unstyled collapse" data-bs-parent="#sidebar">
                    <li><a href="#" class="sidebar-link">Admin</a></li>
                    <li><a href="#" class="sidebar-link">Seller</a></li>
                    <li><a href="#" class="sidebar-link">Customer</a></li>
                    <li><a href="#" class="sidebar-link">Guest</a></li>
                </ul>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-globe2"></i>
                    <span> Translation</span>
                </a>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-play-btn"></i>
                    <span> Education Video</span>
                </a>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-gear"></i>
                    <span> Settings</span>
                </a>
            </li>

            <li class="sidebar-item">
                <a href="#" class="sidebar-link">
                    <i class="bi bi-folder"></i>
                    <span> Content</span>
                </a>
            </li>

        </ul>
    </aside>

    <nav class="navbar-light pe-5 ps-0 pt-2">
        <div class="container-fluid justify-content-between d-flex align-items-center">

            <!-- left -->
            <div class="d-flex align-items-center gap-3">
                <button class="btn  p-0 border-0" type="button"><i class="bi bi-search fs-5"></i></button>
                <button class="btn  p-0 border-0" type="button"><i class="bi bi-grid fs-5"></i></button>
            </div>

            <!-- right -->
            <div class="d-flex align-items-center gap-3" style="margin-right: 230px;">
                <button class="btn  p-0 border-0" type="button"><i class="bi bi-moon fs-5"></i></button>
                <button class="btn  p-0 border-0" type="button"><i class="bi bi-bell fs-5"></i></button>
                <button class="btn  p-0 border-0" type="button"><img src="@/assets/united k.jpg" alt="uk flag" style="height: 27px;"></button>

                <div class="dropdown">
                    <button class="btn p-0 border-0 dropdown-toggle" type="button" data-bs-toggle="dropdown">
                        <img src="@/assets/avatar.svg" class="mt-0" alt="User" style="height: 34px;">
                    </button>
                    <ul class="dropdown-menu dropdown-menu-end">
                        <li><a class="dropdown-item" href="#">Profile</a></li>
                        <li><a class="dropdown-item" href="#">Logout</a></li>
                        <li>
                            <hr class="dropdown-divider">
                        </li>
                        <li><a class="dropdown-item text-danger" href="#">Settings</a></li>
                    </ul>
                </div>
            </div>
        </div>
    </nav>
</div>
</template>

<script>

</script>

<style>
#sidebar {
    position: fixed;
    top: 0;
    left: 0;
    width: 200px;
    /* Adjust width as needed */
    height: 100vh;
    overflow-y: auto;
    transition: all 0.3s ease;
}

nav {
    width: 100%;
    position: fixed;
    top: 0;
    left: 250px;
    /* Adjust to match sidebar width */
    right: 0;
    height: 60px;
    /* Adjust height as needed */
    z-index: 1000;
}

.logo-header {
    display: flex;
    align-items: center;
    gap: 12px;
    margin-bottom: 14px;
    margin-top: 10px;
    margin-left: 11px
}

.logo {
    height: 50px;
}

.team-text {
    font-size: 16px;
    font-weight: bold;
    color: #333;
}

a {
    text-decoration: none;
}

.sidebar-nav {
    flex: 1 1 auto;
}

a.sidebar-link {
    color: #333;
    position: relative;
    transition: all 0.35s;
    display: block;
    height: 35px;
    padding: 6px;
    padding-left: 13px;
}

a.sidebar-link:hover {
    background-color: #635BFF;
    color: white;
    border-radius: 10px;
}

.sidebar-link[data-bs-toggle="collapse"]::after {
    border: solid;
    border-width: 0 0.075rem 0.075rem 0;
    content: "";
    display: inline-block;
    padding: 2px;
    position: absolute;
    right: 2rem;
    top: 0.888rem;
    transform: rotate(-135deg);
    transition: all 0.2s ease-out;
}

.sidebar-link[data-bs-toggle="collapse"].collapsed::after {
    transform: rotate(45deg);
    transition: all 0.2s ease-out;
}

.sidebar-item {
    border-radius: 10px;
}

hr {
    width: 180px;
    color: grey;
}
</style>
