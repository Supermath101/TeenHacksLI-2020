<style>
    #page-title {
        text-transform: uppercase;
    }
</style>

<div id="page-title">Forgot Your Password?</div>
<form on:submit|preventDefault={() => alert("Password Submit Button was Clicked!!")}>
    <input id="email-input" type="email" />
</form>
