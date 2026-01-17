<template>
  <q-page class="bg-black text-white">
    <!-- Hero Section -->
    <div class="hero-section relative-position flex flex-center">
      <div class="absolute-full overflow-hidden">
        <q-img src="~assets/hero-bg.jpg" class="fit" style="opacity: 0.4" />
        <div class="absolute-full bg-gradient" />
      </div>

      <div
        class="container relative-position text-center q-pa-md"
        style="max-width: 800px; z-index: 10"
      >
        <h1 class="text-h2 text-weight-bolder q-mb-md">
          Manage Your Customers with <span class="text-gradient">Precision</span>
        </h1>
        <p class="text-h5 text-grey-4 q-mb-xl">
          The ultimate platform for modern businesses to track, analyze, and grow their customer
          base.
        </p>
        <div class="q-gutter-md">
          <q-btn
            unelevated
            color="primary"
            size="lg"
            label="Get Started Now"
            no-caps
            icon-right="arrow_forward"
          />
          <q-btn outline color="white" size="lg" label="View Demo" no-caps />
        </div>
      </div>
    </div>

    <!-- Features Section -->
    <section class="q-py-xl q-px-md">
      <div class="text-center q-mb-xl">
        <h2 class="text-h3 text-weight-bold q-mb-sm">Why Choose Us?</h2>
        <div class="text-red q-mb-md text-uppercase text-weight-bold tracking-wide">
          Key Features
        </div>
      </div>

      <div
        class="row q-col-gutter-lg justify-center container"
        style="max-width: 1200px; margin: 0 auto"
      >
        <div class="col-12 col-md-4">
          <q-card class="glass-card full-height q-pa-md text-center no-shadow">
            <q-card-section>
              <q-icon name="insights" color="red" size="4rem" class="q-mb-md" />
              <div class="text-h5 text-weight-bold q-mb-sm">Advanced Analytics</div>
              <div class="text-grey-4">
                Deep dive into customer behavior with our AI-powered analytics dashboard.
              </div>
            </q-card-section>
          </q-card>
        </div>
        <div class="col-12 col-md-4">
          <q-card class="glass-card full-height q-pa-md text-center no-shadow">
            <q-card-section>
              <q-icon name="security" color="red" size="4rem" class="q-mb-md" />
              <div class="text-h5 text-weight-bold q-mb-sm">Bank-Grade Security</div>
              <div class="text-grey-4">
                Your data is protected by state-of-the-art encryption and security protocols.
              </div>
            </q-card-section>
          </q-card>
        </div>
        <div class="col-12 col-md-4">
          <q-card class="glass-card full-height q-pa-md text-center no-shadow">
            <q-card-section>
              <q-icon name="bolt" color="red" size="4rem" class="q-mb-md" />
              <div class="text-h5 text-weight-bold q-mb-sm">Lightning Fast</div>
              <div class="text-grey-4">
                Optimized for performance to ensure zero lag in your daily operations.
              </div>
            </q-card-section>
          </q-card>
        </div>
      </div>
    </section>

    <!-- Call to Action -->
    <section class="q-py-xl text-center relative-position">
      <div class="container q-pa-md">
        <h2 class="text-h3 text-weight-bold q-mb-lg">Ready to transform your business?</h2>
        <q-btn
          unelevated
          color="primary"
          size="xl"
          label="Join for Free"
          no-caps
          rounded
          class="q-px-xl"
        />
      </div>
    </section>

    <!-- Contact & Footer Section -->
    <footer
      class="bg-black text-white q-py-xl"
      style="border-top: 1px solid rgba(255, 255, 255, 0.1)"
    >
      <div class="container q-pa-md">
        <div class="row justify-center q-mb-lg">
          <div class="text-center">
            <h3 class="text-h4 text-weight-bold q-mb-md">Contact Us</h3>
            <div class="q-gutter-md q-mb-lg">
              <div class="flex flex-center q-gutter-x-md text-h6 text-grey-4">
                <div class="flex flex-center">
                  <q-icon name="email" color="red" size="sm" class="q-mr-sm" />
                  <span>mybusiness@info.com</span>
                </div>
                <div class="flex flex-center">
                  <q-icon name="phone" color="red" size="sm" class="q-mr-sm" />
                  <span>+94 70 245 4973</span>
                </div>
              </div>
            </div>

            <div class="q-gutter-md">
              <q-btn
                round
                flat
                color="white"
                icon="fab fa-facebook"
                type="a"
                href="https://facebook.com"
                target="_blank"
              />
              <q-btn
                round
                flat
                color="white"
                icon="fab fa-instagram"
                type="a"
                href="https://instagram.com"
                target="_blank"
              />
              <q-btn
                round
                flat
                color="white"
                icon="fab fa-youtube"
                type="a"
                href="https://youtube.com"
                target="_blank"
              />
            </div>
          </div>
        </div>
      </div>
    </footer>
  </q-page>
</template>

<style scoped>
.hero-section {
  min-height: 100vh;
  position: relative;
}

.bg-gradient {
  background: linear-gradient(to bottom, transparent 0%, #000000 100%);
}

.tracking-wide {
  letter-spacing: 2px;
}
</style>

<script setup></script>
