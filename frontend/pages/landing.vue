<template>
  <section class="my-3 p-3 bg-white rounded box-shadow" >
    <div class="alert alert-success" role="alert">
      <small><strong>Well done!</strong> Aww yeah, you successfullying logged in.<br/>
        Your SAML 2.0 authentication process works fine.</small>
    </div>
    <p><img class="img-fluid" src="/static/img/nyan-cat.png" /></p>
    <p>You are logged as <span class="badge badge-dark" text="${username}">null</span>.</p>
    <small class="d-block text-right mt-3" id="sso-btn">
      <nuxt-link to="/saml/logout" class="btn btn-spring btn-sm">
        <i class="far fa-user-circle"></i> Global logout
      </nuxt-link>
      <nuxt-link to="/saml/logout?local=true" class="btn btn-spring btn-sm">
        <i class="fas fa-sign-out-alt"></i> Local logout
      </nuxt-link>
    </small>
  </section>
</template>
