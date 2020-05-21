<template>
  <section class="my-3 p-3 bg-white rounded box-shadow">
    <div class="alert alert-warning" role="alert">
      <small>
        <strong>Here we go!</strong> Select an Identity provider that holds your authentication data.<br/>
        <img class="img-fluid margin-top-10 margin-bottom-10" src="/static/img/saml-flow.png" />
        The Service Provider (SP) generates a SAML 2.0 authentication request, which is encoded and embedded into the URL for SSO
        service. After being redirected, you must provide your credentials to authenticate against the selected IdP.</small>
    </div>

    <h6 class="border-bottom border-gray pb-2 mb-0">Select your Identity Provider:</h6>

    <form action="${idpDiscoReturnURL}" method="get">
      <fieldset class="form-group">
        <div class="form-check" each="idp : ${idps}">
          <label class="form-check-label">
            <input type="radio" class="form-check-input" name="${idpDiscoReturnParam}" id="'idp_' + ${idp}" value="${idp}" />
            <span class="badge badge-dark" text="${idp}">null</span>
          </label>
        </div>
      </fieldset>

      <small class="d-block text-right mt-3" id="sso-btn">
        <button type="submit" class="btn btn-spring btn-sm">
          <i class="fas fa-handshake"></i> Start 3rd Party Login
        </button>
      </small>
    </form>
  </section>
</template>
<script>
export default {

}
</script>
