<template>
  <div>
    <app-tabs>
    <app-tab name="Login" :selected="true">
      <app-card>
        <login-form></login-form>
      </app-card>
    </app-tab>
    <app-tab name="Register">
      <app-card>
        <register-form></register-form>
      </app-card>
    </app-tab>
    </app-tabs>
  </div>
</template>

<script>
import AppTab from '@/components/Tabs/AppTab'
import AppTabs from '@/components/Tabs/AppTabs'
import AppCard from '@/components/AppCard'
import RegisterForm from '@/components/RegisterForm'
import LoginForm from '@/components/LoginForm'
export default {
  components: {
    AppTab,
    AppTabs,
    AppCard,
    RegisterForm,
    LoginForm
  }
}
</script>

<style></style>
