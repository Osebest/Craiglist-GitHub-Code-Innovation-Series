<script setup>
import { ref } from "vue"

const show1 = ref(false)
const show2 = ref(false)
const show3 = ref(false)
const show4 = ref(false)
const show5 = ref(false)
const show6 = ref(false)
const show7 = ref(false)

const th = () =>{
  console.log(Calendar)
}

</script>

<template>
  <div class="bg">
    <v-container>
      <v-row no-gutters>
        <v-col cols="12" sm="3" class="mb-4">
          <div class="flex px-2 pb-2">
            <v-icon icon="mdi-calendar" color="#3E96ED"></v-icon>
            <p class="px-2 text-[#3E96ED] font-semibold">Event Calendar</p>
          </div>
          <div>
            <v-sheet class="d-none d-sm-block m-2 py-2 px-4 mb-4 text-medium-emphasis" rounded>
              <div class="flex items-center mb-2 pt-1">
                <v-icon icon="mdi-account-multiple" color="#3E96ED"></v-icon>
                <p class="px-2 text-[#3E96ED] font-medium">Upcoming Events</p>
              </div>
              <v-divider thickness="3"></v-divider>
              <div class="mt-2">
                <p class="pb-1">Activities</p>
                <p class="pb-1">Childcare</p>
                <p class="pb-1">Classes</p>
                <p class="pb-1">Connections</p>
                <p class="pb-1">General</p>
              </div>
            </v-sheet>
            <v-sheet class="d-sm-none m-2 py-2 px-4 mb-4 text-medium-emphasis" rounded>
              <div class="flex items-center mb-2">
                <v-icon icon="mdi-account-multiple" color="#3E96ED"></v-icon>
                <p class="px-2 text-[#3E96ED] font-medium">Upcoming Events</p>
                <v-spacer></v-spacer>
                <v-icon color="#3E96ED" :icon="show7 ? 'mdi-chevron-up mdi-36px' : 'mdi-chevron-down mdi-36px'"
                  @click="show7 = !show7"></v-icon>
              </div>
              <v-expand-transition>
                <div v-show="show7">
                  <v-divider thickness="3"></v-divider>
                  <div class="mt-2">
                    <p class="pb-1">Activities</p>
                    <p class="pb-1">Childcare</p>
                    <p class="pb-1">Classes</p>
                    <p class="pb-1">Connections</p>
                    <p class="pb-1">General</p>
                  </div>
                </div>
              </v-expand-transition>
            </v-sheet>
          </div>
          <div>
            <v-sheet class="d-none d-sm-block m-2 py-2 px-4 text-medium-emphasis" rounded>
              <div class="flex items-center mb-2 pt-1">
                <v-icon icon="mdi-account-multiple" color="#3E96ED"></v-icon>
                <p class="px-2 text-[#3E96ED] font-medium">Community</p>
              </div>
              <v-divider thickness="3"></v-divider>
              <div class="mt-2">
                <p class="pb-1">Artists</p>
                <p class="pb-1">Activities</p>
                <p class="pb-1">Childcare</p>
                <p class="pb-1">Classes</p>
                <p class="pb-1">Connections</p>
                <p class="pb-1">General</p>
                <p class="pb-1">Groups</p>
                <p class="pb-1">Local News</p>
                <p class="pb-1">Musicians</p>
                <p class="pb-1">Politics</p>
                <p class="pb-1">Rants & Raves</p>
                <p class="pb-1">Rideshare</p>
                <p class="pb-1">Volunteers</p>
              </div>
            </v-sheet>
            <v-sheet class="d-sm-none m-2 py-2 px-4 text-medium-emphasis" rounded>
              <div class="flex items-center mb-2">
                <v-icon icon="mdi-account-multiple" color="#3E96ED"></v-icon>
                <p class="px-2 text-[#3E96ED] font-medium">Community</p>
                <v-spacer></v-spacer>
                <v-icon color="#3E96ED" :icon="show7 ? 'mdi-chevron-up mdi-36px' : 'mdi-chevron-down mdi-36px'"
                  @click="show7 = !show7"></v-icon>
              </div>
              <v-expand-transition>
                <div v-show="show7">
                  <v-divider thickness="3"></v-divider>
                  <div class="mt-2">
                    <p class="pb-1">Artists</p>
                    <p class="pb-1">Activities</p>
                    <p class="pb-1">Childcare</p>
                    <p class="pb-1">Classes</p>
                    <p class="pb-1">Connections</p>
                    <p class="pb-1">General</p>
                    <p class="pb-1">Groups</p>
                    <p class="pb-1">Local News</p>
                    <p class="pb-1">Musicians</p>
                    <p class="pb-1">Politics</p>
                    <p class="pb-1">Rants & Raves</p>
                    <p class="pb-1">Rideshare</p>
                    <p class="pb-1">Volunteers</p>
                  </div>
                </div>
              </v-expand-transition>
            </v-sheet>
          </div>
        </v-col>
        <v-col cols="12" sm="9">
          <h1 class="text-2xl font-bold px-2 mb-2">Explore By Category</h1>

          <v-row no-gutters>
            <v-col cols="12" xs="6" sm="4">
              <v-sheet class="d-none d-sm-block m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2 pt-1">
                  <v-icon icon="mdi-account-key" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Gigs</p>
                </div>
                <v-divider thickness="3"></v-divider>
                <div class="mt-2">
                  <p class="pb-1">Computer</p>
                  <p class="pb-1">Creatives</p>
                  <p class="pb-1">Domestic</p>
                  <p class="pb-1">Events</p>
                  <p class="pb-1">Talent</p>
                  <p class="pb-1">Writing</p>
                </div>
              </v-sheet>
              <v-sheet class="d-sm-none m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2">
                  <v-icon icon="mdi-account-key" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Gigs</p>
                  <v-spacer></v-spacer>
                  <v-icon color="#3E96ED" :icon="show1 ? 'mdi-chevron-up mdi-36px' : 'mdi-chevron-down mdi-36px'"
                    @click="show1 = !show1"></v-icon>
                </div>
                <v-expand-transition>
                  <div v-show="show1">
                    <v-divider thickness="3"></v-divider>
                    <div class="mt-2">
                      <p class="pb-1">Computer</p>
                      <p class="pb-1">Creatives</p>
                      <p class="pb-1">Domestic</p>
                      <p class="pb-1">Events</p>
                      <p class="pb-1">Talent</p>
                      <p class="pb-1">Writing</p>
                    </div>
                  </div>
                </v-expand-transition>
              </v-sheet>
            </v-col>
            <v-col cols="12" xs="6" sm="4" class="sm:mt-4">
              <v-sheet class="d-none d-sm-block m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2 pt-1">
                  <v-icon icon="mdi-briefcase mdi-spin" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Jobs</p>
                </div>
                <v-divider thickness="3"></v-divider>
                <div class="mt-2">
                  <p class="pb-1">Admin / Office</p>
                  <p class="pb-1">Arch / Engineering</p>
                  <p class="pb-1">Education</p>
                  <p class="pb-1">Human Resources</p>
                  <p class="pb-1">Government</p>
                  <p class="pb-1">Manufacturing</p>
                  <p class="pb-1">Security</p>
                  <p class="pb-1">Transport</p>
                  <p class="pb-1">Writing / Editing</p>
                </div>
              </v-sheet>
              <v-sheet class="d-sm-none m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2">
                  <v-icon icon="mdi-briefcase mdi-spin" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Jobs</p>
                  <v-spacer></v-spacer>
                  <v-icon color="#3E96ED" :icon="show2 ? 'mdi-chevron-up mdi-36px' : 'mdi-chevron-down mdi-36px'"
                    @click="show2 = !show2"></v-icon>
                </div>
                <v-expand-transition>
                  <div v-show="show2">
                    <v-divider thickness="3"></v-divider>
                    <div class="mt-2">
                      <p class="pb-1">Admin / Office</p>
                      <p class="pb-1">Arch / Engineering</p>
                      <p class="pb-1">Education</p>
                      <p class="pb-1">Human Resources</p>
                      <p class="pb-1">Government</p>
                      <p class="pb-1">Manufacturing</p>
                      <p class="pb-1">Security</p>
                      <p class="pb-1">Transport</p>
                      <p class="pb-1">Writing / Editing</p>
                    </div>
                  </div>
                </v-expand-transition>
              </v-sheet>
            </v-col>
            <v-col cols="12" xs="6" sm="4" class="sm:mt-8">
              <v-sheet class="d-none d-sm-block m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2 pt-1">
                  <v-icon icon="mdi-home" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Housing</p>
                </div>
                <v-divider thickness="3"></v-divider>
                <div class="mt-2">
                  <p class="pb-1">Apt/Housing</p>
                  <p class="pb-1">House Swap</p>
                  <p class="pb-1">Housing wanted</p>
                  <p class="pb-1">Parking / Storage</p>
                  <p class="pb-1">Real Estate for sale</p>
                  <p class="pb-1">Rooms wanted</p>
                  <p class="pb-1">Rooms / Shared</p>
                  <p class="pb-1">Sublets / Temporary</p>
                  <p class="pb-1">Vacation rental</p>
                </div>
              </v-sheet>
              <v-sheet class="d-sm-none m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2">
                  <v-icon icon="mdi-home" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Housing</p>
                  <v-spacer></v-spacer>
                  <v-icon color="#3E96ED" :icon="show3 ? 'mdi-chevron-up mdi-36px' : 'mdi-chevron-down mdi-36px'"
                    @click="show3 = !show3"></v-icon>
                </div>
                <v-expand-transition>
                  <div v-show="show3">
                    <v-divider thickness="3"></v-divider>
                    <div class="mt-2">
                      <p class="pb-1">Apt/Housing</p>
                      <p class="pb-1">House Swap</p>
                      <p class="pb-1">Housing wanted</p>
                      <p class="pb-1">Parking / Storage</p>
                      <p class="pb-1">Real Estate for sale</p>
                      <p class="pb-1">Rooms wanted</p>
                      <p class="pb-1">Rooms / Shared</p>
                      <p class="pb-1">Sublets / Temporary</p>
                      <p class="pb-1">Vacation rental</p>
                    </div>
                  </div>
                </v-expand-transition>
              </v-sheet>
            </v-col>
            <v-col cols="12" xs="6" sm="4" class="sm:-mt-44 md:-mt-28">
              <v-sheet class="d-none d-sm-block m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2 pt-1">
                  <v-icon icon="mdi-sale mdi-spin" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">For Sale</p>
                </div>
                <v-divider thickness="3"></v-divider>
                <div class="mt-2">
                  <p class="pb-1">Antiques</p>
                  <p class="pb-1">Aviation</p>
                  <p class="pb-1">Business</p>
                  <p class="pb-1">Computer</p>
                  <p class="pb-1">Computer Parts</p>
                  <p class="pb-1">Electronics</p>
                  <p class="pb-1">Household</p>
                  <p class="pb-1">Jewelry</p>
                  <p class="pb-1">Materials</p>
                  <p class="pb-1">Sporting</p>
                  <p class="pb-1">Tickets</p>
                  <p class="pb-1">Video gaming</p>
                </div>
              </v-sheet>
              <v-sheet class="d-sm-none m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2">
                  <v-icon icon="mdi-sale mdi-spin" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">For Sale</p>
                  <v-spacer></v-spacer>
                  <v-icon color="#3E96ED" :icon="show4 ? 'mdi-chevron-up mdi-36px' : 'mdi-chevron-down mdi-36px'"
                    @click="show4 = !show4"></v-icon>
                </div>
                <v-expand-transition>
                  <div v-show="show4">
                    <v-divider thickness="3"></v-divider>
                    <div class="mt-2">
                      <p class="pb-1">Antiques</p>
                      <p class="pb-1">Aviation</p>
                      <p class="pb-1">Business</p>
                      <p class="pb-1">Computer</p>
                      <p class="pb-1">Computer Parts</p>
                      <p class="pb-1">Electronics</p>
                      <p class="pb-1">Household</p>
                      <p class="pb-1">Jewelry</p>
                      <p class="pb-1">Materials</p>
                      <p class="pb-1">Sporting</p>
                      <p class="pb-1">Tickets</p>
                      <p class="pb-1">Video gaming</p>
                    </div>
                  </div>
                </v-expand-transition>
              </v-sheet>
            </v-col>
            <v-col cols="12" xs="6" sm="4" class="sm:-mt-6 md:-mt-4">
              <v-sheet class="d-none d-sm-block m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2 pt-1">
                  <v-icon icon="mdi-message-draw" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Discussion Forum</p>
                </div>
                <v-divider thickness="3"></v-divider>
                <div class="mt-2">
                  <p class="pb-1">Art</p>
                  <p class="pb-1">Atheists</p>
                  <p class="pb-1">Divorce</p>
                  <p class="pb-1">Marriage</p>
                  <p class="pb-1">Money</p>
                  <p class="pb-1">Music</p>
                  <p class="pb-1">Politics</p>
                  <p class="pb-1">Religion</p>
                  <p class="pb-1">Science</p>
                </div>
              </v-sheet>
              <v-sheet class="d-sm-none m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2">
                  <v-icon icon="mdi-message-draw" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Discussion Forum</p>
                  <v-spacer></v-spacer>
                  <v-icon color="#3E96ED" :icon="show5 ? 'mdi-chevron-up mdi-36px' : 'mdi-chevron-down mdi-36px'"
                    @click="show5 = !show5"></v-icon>
                </div>
                <v-expand-transition>
                  <div v-show="show5">
                    <v-divider thickness="3"></v-divider>
                    <div class="mt-2">
                      <p class="pb-1">Art</p>
                      <p class="pb-1">Atheists</p>
                      <p class="pb-1">Divorce</p>
                      <p class="pb-1">Marriage</p>
                      <p class="pb-1">Money</p>
                      <p class="pb-1">Music</p>
                      <p class="pb-1">Politics</p>
                      <p class="pb-1">Religion</p>
                      <p class="pb-1">Science</p>
                    </div>
                  </div>
                </v-expand-transition>
              </v-sheet>
            </v-col>
            <v-col cols="12" xs="6" sm="4">
              <v-sheet class="d-none d-sm-block m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2 pt-1">
                  <v-icon icon="mdi-silverware-variant mdi-spin" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Services</p>
                </div>
                <v-divider thickness="3"></v-divider>
                <div class="mt-2">
                  <p class="pb-1">Automobile</p>
                  <p class="pb-1">Beauty</p>
                  <p class="pb-1">Creative</p>
                  <p class="pb-1">Computer</p>
                  <p class="pb-1">Farm and Garden</p>
                  <p class="pb-1">Financial</p>
                  <p class="pb-1">Legal</p>
                  <p class="pb-1">Pet</p>
                  <p class="pb-1">Real estate</p>
                </div>
              </v-sheet>
              <v-sheet class="d-sm-none m-2 py-2 px-4 text-medium-emphasis" rounded>
                <div class="flex items-center mb-2">
                  <v-icon icon="mdi-silverware-variant mdi-spin" color="#3E96ED"></v-icon>
                  <p class="px-2 text-[#3E96ED] font-medium">Services</p>
                  <v-spacer></v-spacer>
                  <v-icon color="#3E96ED" :icon="show6 ? 'mdi-chevron-up mdi-36px' : 'mdi-chevron-down mdi-36px'"
                    @click="show6 = !show6"></v-icon>
                </div>
                <v-expand-transition>
                  <div v-show="show6">
                    <v-divider thickness="3"></v-divider>
                    <div class="mt-2">
                      <p class="pb-1">Automobile</p>
                      <p class="pb-1">Beauty</p>
                      <p class="pb-1">Creative</p>
                      <p class="pb-1">Computer</p>
                      <p class="pb-1">Farm and Garden</p>
                      <p class="pb-1">Financial</p>
                      <p class="pb-1">Legal</p>
                      <p class="pb-1">Pet</p>
                      <p class="pb-1">Real estate</p>
                    </div>
                  </div>
                </v-expand-transition>
              </v-sheet>
            </v-col>
          </v-row>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<style scoped>
.bg{
  background-color: rgba(0, 0, 0, 0.1);
  margin-top: 20px;
}
</style>