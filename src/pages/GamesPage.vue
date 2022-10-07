<template>
    <q-page>
      <q-card style="width:100%">
        <q-tabs
          v-model="tab"
          class="text-black"
          active-color="white"
          indicator-color="white"
          align="justify"
        >
          <q-tab name="pc" label="PC" />
          <q-tab name="ps" label="PlayStation" />
          <q-tab name="xbox" label="XBox" />
          <q-tab name="nintendo" label="Nintendo" />
        </q-tabs>

        <q-separator />

        <q-tab-panels v-model="tab" animated class="games">
          <q-tab-panel name="pc">
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/PJTcM2FQ/Crysis3.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Crysis 3 Remastered</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/mg467dJX/Dark-Souls-1.webp"/>
              <q-card-section>
                <div class="text-overline text-center overline">Dark Souls 1 Remastered</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/6pdqmQH6/Cod-4jpeg.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">CoD 4 Modern Warfare</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/nzLvxm5G/Fable-iii.webp"/>
              <q-card-section>
                <div class="text-overline text-center overline">Fable III</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/2ys99YGv/Dying-Light-cover.webp"/>
              <q-card-section>
                <div class="text-overline text-center overline">Dying light</div>
              </q-card-section>
            </q-card>
          </q-tab-panel>

          <q-tab-panel name="ps">
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/WbqL8zbh/Horizon-Zero-Dawn.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Horizon Zero Dawn</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/RVW6T7HK/The-Last-of-Us.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">The Last of Us Part II</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/BZHQZmHh/Uncharted-4.webp"/>
              <q-card-section>
                <div class="text-overline text-center overline">Uncharted 4</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/9MHKLY0M/infamous.webp"/>
              <q-card-section>
                <div class="text-overline text-center overline">inFamous Second Son</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/bvy2kKHN/Nioh-The-Complete-Edition.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Nioh</div>
              </q-card-section>
            </q-card>
          </q-tab-panel>

          <q-tab-panel name="xbox">
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/6pnsJpST/dead-rising-3.webp"/>
              <q-card-section>
                <div class="text-overline text-center overline">Dead Rising 3</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/pr0hDnFd/Ryse.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Ryse Son of Rome</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/cHt0Dg2H/Q-Break.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Quantam Break</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/bJh354Ft/Sunset-Overdrive.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Sunset Overdrive</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/W3qqM47m/Halo.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Halo Infinite</div>
              </q-card-section>
            </q-card>
          </q-tab-panel>

          <q-tab-panel name="nintendo">
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/RCWVkkK2/the-legend-of-zelda-breath-of-the-wildjpeg.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">LoZ Breath Of The Wild</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/qqpfvCgm/Mario-Party-Super-Stars.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Mario Party Superstars</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/x8j0FZGT/MH-Rise.jpg"/>
              <q-card-section>
                <div class="text-overline text-center overline">Monster Hunter Rise</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/GmpJF3ZH/Hinokami.webp"/>
              <q-card-section>
                <div class="text-overline text-center overline">Demon Slayer The Hinokami Chronicles</div>
              </q-card-section>
            </q-card>
            <q-card class="game q-ma-lg" flat bordered square>
              <q-img src="https://i.postimg.cc/zXf14MM4/Smash-Bros-1.png"/>
              <q-card-section>
                <div class="text-overline text-center overline">Super Smash Bros. Ultimate</div>
              </q-card-section>
            </q-card>
          </q-tab-panel>
        </q-tab-panels>
      </q-card>

    </q-page>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      tab: ref('pc')
    }
  }
}

</script>

<style>
  .q-tabs{
    background: linear-gradient(#5408E6,#DD1931);
    border-radius: 0;
  }

  .q-tab{
    border-radius: 0;
  }

  .q-tab-panels{
    display: flex !important;
    flex-flow: row wrap;
    justify-content: center;
    background: url('https://i.postimg.cc/nhKmhwvh/wp5633980-neon-aesthetic-4k-wallpapers.jpg')no-repeat center center/cover;
  }
  .game{
    max-width: 400px;
    min-width: 400px;
  }
  .q-tab-panel{
    display: flex !important;
    flex-flow: row wrap;
    justify-content: center;
  }

  .overline{
    font-size: 15px;
  }

</style>
