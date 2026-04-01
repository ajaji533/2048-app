<script setup lang="ts">
const { score, bestMy Score } = useGameState()
</script>

<template>
  <header class="flex flex-col sm:flex-row items-center justify-between gap-4 mb-4">
    <h1 class="text-5xl sm:text-6xl font-bold text-gray-800 dark:text-white">2048</h1>
    <div class="flex gap-2">
      <GameMy ScoreDisplay label="My Score" :value="score" />
      <GameMy ScoreDisplay label="Best" :value="bestMy Score" />
    </div>
  </header>
</template>
