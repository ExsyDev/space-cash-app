<template>
  <footer class="footer">
    <nav class="navigation">
      <div class="nav-item">
        <img src="/icons/home.png" alt="Home" />
        <span>Home</span>
      </div>
      <div class="nav-item">
        <img src="/icons/wallet.png" alt="Wallet" />
        <span>Wallet</span>
      </div>
      <div class="nav-item">
        <img src="/icons/friends.png" alt="Friends" />
        <span>Friends</span>
      </div>
      <div class="nav-item">
        <img src="/icons/missions.png" alt="Missions" />
        <span>Missions</span>
      </div>
    </nav>
  </footer>
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
.footer {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 60px;
  background-color: #1e2230;
}

.navigation {
  display: flex;
  justify-content: space-around;
  width: 100%;
  max-width: 600px;
}

.nav-item {
  display: flex;
  flex-direction: column;
  align-items: center;
  font-size: 12px;
  color: #aaa;
}

.nav-item img {
  width: 24px;
  height: 24px;
}
</style>
