<template>
  <!-- 使用表格布局实现等高列 -->
  <div>
    <header>
      <h1>Franklin Running Club</h1>
    </header>
    <div class="wrapper">
      <div class="container">
        <main class="main">
          <h2>Come join us!</h2>
          <p>
            The Franklin Running club meets at 6:00pm every Thursday
            at the town square. Runs are three to five miles, at your
            own pace.
          </p>
        </main>
        <aside class="sidebar">
          <div class="widget"></div>
          <div class="widget"></div>
          <div class="gizmo"></div>
        </aside>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "ContourColumnTable"
}
</script>

<style scoped>

body {
  background-color: #eee;
  font-family: Helvetica, Arial, sans-serif;
}

.container {
  display: table;
  width: 100%;
  border-spacing: 1.5em 0;
}

header {
  color: #fff;
  background-color: #0072b0;
  border-radius: .5em;
}

.main {
  display: table-cell;
  width: 70%;
  background-color: #ad9a9a;
  border-radius: .5em;
}

.wrapper {
  margin-left: -1.5em;
  margin-right: -1.5em;
}

.sidebar {
  display: table-cell;
  width: 30%;
  /*margin-left: 1.5em; 外边距不再生效 */
  padding: 1.5em;
  background-color: #ad9a9a;
  border-radius: .5em;
}
</style>
