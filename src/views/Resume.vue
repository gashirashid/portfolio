<template>
  <v-layout row justify-center align-center wrap class="mt-4 pt-2">
    <v-flex xs12 sm12 md5 lg6 xl6 class="mt-4 pt-4">
      <h2 class="mb-4 pl-4 pt-2">Education</h2>
      <v-card-text class="py-0">
        <v-timeline align-top dense>
          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">AUG 2016 -</div>
                <div class="caption font-weight-bold green--text">NOV 2020</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Bachelor Of Technology with 80%</strong>
                <div class="caption mb-2">University Of Kashmir  </div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">DEC 2014 -</div>
                <div class="caption font-weight-bold green--text">NOV 2015</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>12th with 73.2%</strong>
                <div class="caption mb-2">JK BOSE </div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">DEC 2012 -</div>
                <div class="caption font-weight-bold green--text">NOV 2013</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>10th with 82.8%</strong>
                <div class="caption mb-2">JK BOSE </div>
              </v-flex>
            </v-layout>
          </v-timeline-item>
        </v-timeline>
      </v-card-text>
    </v-flex>
    <v-flex xs12 sm12 md4 lg6 xl6 class="mt-4 pt-2">
      <h2 class="mb-4 pl-4">Experience</h2>
      <v-card-text class="py-0">
        <v-timeline align-top dense>
          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">NOV 2021 -</div>
                <div class="caption font-weight-bold green--text">JUNE 2022</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Sr. PHP Developer</strong>
                <div class="caption mb-2">LBM SOLUTIONS MOHALI</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">JAN 2021 -</div>
                <div class="caption font-weight-bold green--text">NOV 2021</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Junior PHP Developer</strong>
                <div class="caption mb-2">LBM SOLUTIONS MOHALI</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>

          <v-timeline-item color="green" small>
            <v-layout pt-3>
              <v-flex xs4>
                <div class="caption font-weight-bold green--text">OCT 2019 -</div>
                <div class="caption font-weight-bold green--text">FEB 2020</div>
              </v-flex>
              <v-flex class="pl-2">
                <strong>Web Developer Intern</strong>
                <div class="caption mb-2">Ready Steady Digital</div>
              </v-flex>
            </v-layout>
          </v-timeline-item>
        </v-timeline>
      </v-card-text>
    </v-flex>
    <v-layout row justify-center align-center wrap class="mt-4 pt-2">
      <v-flex xs12 sm12 md4 lg5 xl5 class="mx-2 pt-4">
        <h2>
          <span>Design</span>

          <span class="green--text">Skills</span>
        </h2>
        <br>
        <strong>BOOTSTRAP</strong>
        <v-progress-linear v-model="buffer1" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>CSS</strong>
        <v-progress-linear v-model="buffer2" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>VUE JS</strong>
        <v-progress-linear v-model="buffer3" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
      </v-flex>
      <v-flex xs12 sm12 md4 lg5 xl5 class="mx-2 pt-4">
        <h2>
          <span>Coding</span>
          <span class="green--text">Skills</span>
        </h2>
        <br>
        <strong>PHP</strong>
        <v-progress-linear v-model="buffer4" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>LARAVEL/CODEIGNITER</strong>
        <v-progress-linear v-model="buffer5" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
        <strong>JAVASCRIPT</strong>
        <v-progress-linear v-model="buffer6" :buffer-value="bufferValue" color="green" height="16"></v-progress-linear>
      </v-flex>
      <div class="mt-4 pt-2">
        <v-btn
          href="https://drive.google.com/file/d/1nSuz-3tx8PhFKyXo1oRZ9hVMhkJHiZxn/view?usp=sharing"
          target="_blank"
          color="green"
          dark
          large
        >
          Download Resume
          <v-icon right dark>fas fa-file-download</v-icon>
        </v-btn>
      </div>
    </v-layout>
  </v-layout>
</template>

<script>
export default {
  metaInfo: {
    title: "Resume",
    titleTemplate: "%s ← Yaseen's Rashid",
    meta: [
      { name: "viewport", content: "width=device-width, initial-scale=1" },
      {
        name: "description",
        content:
          "PHP Laravel Codeigniter Vue js  javascript web developer"
      },
      { charset: "utf-8" },
      { property: "og:title", content: "Yaseen' Rashid" },
      { property: "og:site_name", content: "Yaseen' Rashid" },
      { property: "og:type", content: "website" },
      { property: "og:url", content: "https://Yaseen.Rashid" },
      {
        property: "og:image",
        content: "https://i.imgur.com/Dcz2PGx.jpg"
      },
      {
        property: "og:description",
        content:
          "PHP Laravel Codeigniter Vue js  javascript web developer"
      }
    ]
  },
  data() {
    return {
      value: 0,
      buffer1: 0,
      buffer2: 0,
      buffer3: 0,
      buffer4: 0,
      buffer5: 0,
      buffer6: 0,
      bufferValue: 100,
      interval: 0
    };
  },
  mounted() {
    this.startBuffer();
  },

  beforeDestroy() {
    clearInterval(this.interval);
  },

  methods: {
    startBuffer() {
      this.interval = setInterval(() => {
        this.buffer1 = 90;
        this.buffer2 = 85;
        this.buffer3 = 80;
        this.buffer4 = 90;
        this.buffer5 = 80;
        this.buffer6 = 82;
      }, 800);
    }
  }
};
</script>
<style >
</style>

