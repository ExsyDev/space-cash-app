<template>
  <div class="main-content">
    <div class="profile-section">
      <div class="rank-list">
        <div class="rank-item" v-for="rank in ranks" :key="rank">{{ rank }}</div>
      </div>
      <div class="profile-image">
        <img src="/profile.jpg" alt="Profile" />
      </div>
    </div>
    <div class="stats-section">
      <p class="uni-balance">4.758252 UNI</p>
      <p class="ghs-rate">1.0 GH/S</p>
    </div>
    <div class="actions">
      <button class="btn claim-btn">CLAIM</button>
      <button class="btn boost-btn">BOOST</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ranks: ['RANG 1', 'RANG 2', 'RANG 3', 'RANG 4', 'RANG 5']
    }
  }
}
</script>

<style scoped>
.main-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 20px;
}

.profile-section {
  display: flex;
  align-items: center;
  margin-bottom: 20px;
}

.rank-list {
  margin-right: 20px;
}

.rank-item {
  margin: 5px 0;
  color: #aaa;
}

.profile-image img {
  border-radius: 50%;
  width: 100px;
  height: 100px;
}

.stats-section {
  text-align: center;
  margin-bottom: 20px;
}

.uni-balance {
  font-size: 24px;
  font-weight: bold;
}

.ghs-rate {
  font-size: 14px;
  color: #999;
}

.actions {
  display: flex;
  gap: 10px;
}

.btn {
  padding: 10px 20px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.claim-btn {
  background-color: #fff;
  color: #000;
}

.boost-btn {
  background-color: #ff6600;
  color: #fff;
}
</style>
