<template>
  <div id="app">
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
  <a class="navbar-brand" href="#">Navbar</a>
  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavDropdown" aria-controls="navbarNavDropdown" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>
  <div class="collapse navbar-collapse" id="navbarNavDropdown">
    <ul class="navbar-nav">
      <!-- dropdown #1 시작 -->
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          About
        </a>
        <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
          <router-link to="/home" class="dropdown-item">
            Home
          </router-link>
          <router-link to="/complain" class="dropdown-item">
            Complain
          </router-link>
        </div>
      </li>
      <!-- dropdown #1 끝 -->

      <!-- dropdown #2 시작 -->
      <li class="nav-item dropdown">
        <a class="nav-link dropdown-toggle" href="#" id="navbarDropdownMenuLink" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
          Tutorial menu
        </a>
        <div class="dropdown-menu" aria-labelledby="navbarDropdownMenuLink">
          <router-link to="/tutorial" class="dropdown-item">
            Home
          </router-link>
          <router-link to="/add" class="dropdown-item">
            Add
          </router-link>
        </div>
      </li>
      <!-- dropdown #2 끝 -->
    </ul>
  </div>
</nav>
    <!-- nav 시작 -->
    <!-- <nav class="navbar navbar-expand navbar-dark bg-dark"> -->
      <!-- <router-link to="/" class="navbar-brand"> -->
        <!-- bezkoder -->
      <!-- </router-link> -->
      <!-- div 시작 -->
      <!-- <div class="navbar-nav mr-auto"> -->
        <!-- <li class="nav-item"> -->
          <!-- <router-link to="/tutorials" class="nav-link"> -->
            <!-- Tutorials -->
          <!-- </router-link> -->
        <!-- </li> -->
        <!-- <li class="nav-item"> -->
          <!-- <router-link to="/add" class="nav-link"> -->
            <!-- Add -->
          <!-- </router-link> -->
        <!-- </li> -->
      <!-- </div> -->
      <!-- div 끝 -->
    <!-- </nav>  -->
    <!-- nav 끝 -->
    <div class="container mt-3">
      <!-- 위의 router-link 있는 메뉴 화면이 아래위치에 표시 -->
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
export default {
  name: "app"
}
</script>

<style>

</style>