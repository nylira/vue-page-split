# vue-page-split
Header and content split page component for Vue 2.

## Installation

    npm install @nylira/vue-page-split

## Usage

    <template>
      <page-split>
        <header>Just a cool header!</header>
        <div class="body">Just some body text.</div>
      </page-split>
    </template>

    <script>
      import PageSplit from '@nylira/vue-page-split'
      export default {
        components: {
          PageSplit
        }
      }
    </script>

    <style>
      .ni-page-split {
        background: #f00;
      }
    </style>
