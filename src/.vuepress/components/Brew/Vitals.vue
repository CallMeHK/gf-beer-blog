<template>
<div>
  <table class='mobile'>
    <tbody>
      <tr>
        <th>OG</th>
        <td>{{ og }}</td>
      </tr>
      <tr>
        <th>FG</th>
        <td>{{ fg }}</td>
      </tr>
      <tr>
        <th>ABV</th>
        <td>{{ abv }}</td>
      </tr>
      <tr>
        <th>IBU</th>
        <td>{{ ibu }}</td>
      </tr>
      <tr>
        <th>SRM</th>
        <td>{{ srm }}</td>
      </tr>
      <tr>
        <th>Efficiency</th>
        <td>{{ eff }}</td>
      </tr>
    </tbody>
  </table>
  <table class="desktop">
    <thead>
      <tr>
        <th>OG</th>
        <th>FG</th>
        <th>ABV</th>
        <th>IBU</th>
        <th>SRM</th>
        <th>Efficiency</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <td>{{ og }}</td>
        <td>{{ fg }}</td>
        <td>{{ abv }}</td>
        <td>{{ ibu }}</td>
        <td>{{ srm }}</td>
        <td>{{ eff }}</td>
      </tr>
    </tbody>
  </table>
</div>
</template>

<script>
  export default {
    props: {
      og: { required: true },
      fg: { required: true },
      abv: { required: true },
      ibu: { required: true },
      srm: { required: true },
      eff: { required: true }
    }
  }
</script>

<style scoped>
@media screen and (min-width: 600px) {
  .mobile {
    display: none
  }
}

@media screen and (max-width: 599px) {
  .desktop {
    display: none
  }
}
</style>
