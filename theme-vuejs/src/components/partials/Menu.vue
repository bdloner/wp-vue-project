<template>
  <div v-if="menu" class="main-menu">
    <div class="site-logo">
      <a :href="'/vueproject/'">
        <img class="site-logo-img"
          v-bind:src="'../vueproject/wp-content/uploads/2019/09/site-logo.png'"
        />
      </a>
    </div>
    <div class="menu-bar-desktop">
      <ul class="menu-bar-desktop-ul">
        <li class="menu-bar-desktop-li" v-for="item in menu.items" :key="`menu_item_${item.ID}`">
          <router-link :to="getURLPath(item.url)">{{ item.title }}</router-link>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  props: ["menu"],

  methods: {
    getURLPath(url) {
      var m = url.match(
          /^(([^:\/?#]+:)?(?:\/\/((?:([^\/?#:]*):([^\/?#:]*)@)?([^\/?#:]*)(?::([^\/?#:]*))?)))?([^?#]*)(\?[^#]*)?(#.*)?$/
        ),
        r = {
          hash: m[10] || "", // #asd
          host: m[3] || "", // localhost:257
          hostname: m[6] || "", // localhost
          href: m[0] || "", // http://username:password@localhost:257/deploy/?asd=asd#asd
          origin: m[1] || "", // http://username:password@localhost:257
          pathname: m[8] || (m[1] ? "/" : ""), // /deploy/
          port: m[7] || "", // 257
          protocol: m[2] || "", // http:
          search: m[9] || "", // ?asd=asd
          username: m[4] || "", // username
          password: m[5] || "" // password
        };

      return r.pathname;
    }
  }
};
</script>