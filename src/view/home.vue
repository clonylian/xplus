<template>
  <div class="ymain">
    <div class="yhead">
      <div class="yheadbox flex jus">
        <div class="yheadbleft flex">
          <a href="#">
            <img src="../assets/logo.6d4c186.svg" alt="" />
          </a>
          <div class="yheadbltab flex">
            <a
              @click="activetab('1')"
              :class="headtab == '1' ? 'yheadtabactive' : ''"
              href="#Social"
              >X-Social</a
            >
            <a
              @click="activetab('2')"
              :class="headtab == '2' ? 'yheadtabactive' : ''"
              href="#FOMO"
              >X-FOMO</a
            >
            <a
              @click="activetab('3')"
              :class="headtab == '3' ? 'yheadtabactive' : ''"
              href="#Wallet"
              >X-Wallet</a
            >
            <a
              @click="activetab('4')"
              :class="headtab == '4' ? 'yheadtabactive' : ''"
              href="#Space"
              >X-Space</a
            >
            <a href="https://www.xplus.com/partner">Partnerships</a>
            <a target="_blank" href="https://blog.xplus.com/">Blog</a>
          </div>
        </div>
        <div class="yheadbright flex">
          <a
            class="flex"
            target="_blank"
            href="https://xplus.gitbook.io/xplus/introduction/xplus"
            >DOCS</a
          >
          <div class="yheadbrgj">
            <span></span>
          </div>
        </div>
      </div>
    </div>
    <div class="yone section section-banner">
      <div class="layer-bg">
        <ol class="clips-box">
          <li class="item-phone">
            <div
              class="clip-wrap clip-rect"
              style="clip-path: url('#clipPathBannerRect')"
            >
              <svg
                width="1000"
                height="390"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <rect
                    id="shapeBannerRect"
                    width="1000"
                    height="390"
                    rx="195"
                  ></rect>
                  <clipPath id="clipPathBannerRect">
                    <use xlink:href="#shapeBannerRect"></use>
                  </clipPath>
                </defs>
                <use xlink:href="#shapeBannerRect" class="shape-stroke"></use>
              </svg>
            </div>
            <div class="phone-hand">
              <img
                src="../assets/banner_hand_beside.96c2f5b.png"
                alt=""
                class="img-hand-beside"
              />
              <img
                src="../assets/banner_hand_phone.a7655e1.gif"
                alt=""
                class="img-hand-phone"
              />
            </div>
          </li>
          <li class="item-triangle">
            <div
              class="clip-wrap clip-triangle"
              style="clip-path: url('#clipBannerTriangle')"
            >
              <svg
                width="360"
                height="360"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <path
                    id="shapeBannerTriangle"
                    transform="rotate(-15 180 180)"
                    d="M6.56,246.25,138.63,17.5a30,30,0,0,1,52,0L322.66,246.25a30,30,0,0,1-26,45H32.54A30,30,0,0,1,6.56,246.25Z"
                  ></path>
                  <clipPath id="clipBannerTriangle">
                    <use xlink:href="#shapeBannerTriangle"></use>
                  </clipPath>
                </defs>
                <use
                  xlink:href="#shapeBannerTriangle"
                  class="shape-stroke"
                ></use>
              </svg>
            </div>
          </li>
        </ol>
        <ol
          class="bg-triangles-box"
          style="
            translate: none;
            rotate: none;
            scale: none;
            transform: translate(0px, 0px);
          "
        >
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDIuMDYiIGhlaWdodD0iNDMuNzYiIHZpZXdCb3g9IjAgMCA0Mi4wNiA0Mi43NiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiA+PGRlZnM+PHN0eWxlPi5jbHMtMXtmaWxsOiM5YjliOWI7fTwvc3R5bGU+PC9kZWZzPjxnIGlkPSLlm77lsYJfMiIgZGF0YS1uYW1lPSLlm77lsYIgMiI+PGcgaWQ9ImJhY2tncm91bmQiPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTM2LjUsMzRsLTI2LDguMzdBOCw4LDAsMCwxLC4xOSwzMy4wNkw2LDYuMzJBOCw4LDAsMCwxLDE5LjE1LDIuMDhMMzkuNDMsMjAuNDVBOCw4LDAsMCwxLDM2LjUsMzRaIi8+PC9nPjwvZz48L3N2Zz4="
              alt=""
            />
          </li>
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDIuMDYiIGhlaWdodD0iNDMuNzYiIHZpZXdCb3g9IjAgMCA0Mi4wNiA0Mi43NiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiA+PGRlZnM+PHN0eWxlPi5jbHMtMXtmaWxsOiM5YjliOWI7fTwvc3R5bGU+PC9kZWZzPjxnIGlkPSLlm77lsYJfMiIgZGF0YS1uYW1lPSLlm77lsYIgMiI+PGcgaWQ9ImJhY2tncm91bmQiPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTM2LjUsMzRsLTI2LDguMzdBOCw4LDAsMCwxLC4xOSwzMy4wNkw2LDYuMzJBOCw4LDAsMCwxLDE5LjE1LDIuMDhMMzkuNDMsMjAuNDVBOCw4LDAsMCwxLDM2LjUsMzRaIi8+PC9nPjwvZz48L3N2Zz4="
              alt=""
            />
          </li>
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDIuMDYiIGhlaWdodD0iNDMuNzYiIHZpZXdCb3g9IjAgMCA0Mi4wNiA0Mi43NiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiA+PGRlZnM+PHN0eWxlPi5jbHMtMXtmaWxsOiM5YjliOWI7fTwvc3R5bGU+PC9kZWZzPjxnIGlkPSLlm77lsYJfMiIgZGF0YS1uYW1lPSLlm77lsYIgMiI+PGcgaWQ9ImJhY2tncm91bmQiPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTM2LjUsMzRsLTI2LDguMzdBOCw4LDAsMCwxLC4xOSwzMy4wNkw2LDYuMzJBOCw4LDAsMCwxLDE5LjE1LDIuMDhMMzkuNDMsMjAuNDVBOCw4LDAsMCwxLDM2LjUsMzRaIi8+PC9nPjwvZz48L3N2Zz4="
              alt=""
            />
          </li>
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDIuMDYiIGhlaWdodD0iNDMuNzYiIHZpZXdCb3g9IjAgMCA0Mi4wNiA0Mi43NiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiA+PGRlZnM+PHN0eWxlPi5jbHMtMXtmaWxsOiM5YjliOWI7fTwvc3R5bGU+PC9kZWZzPjxnIGlkPSLlm77lsYJfMiIgZGF0YS1uYW1lPSLlm77lsYIgMiI+PGcgaWQ9ImJhY2tncm91bmQiPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTM2LjUsMzRsLTI2LDguMzdBOCw4LDAsMCwxLC4xOSwzMy4wNkw2LDYuMzJBOCw4LDAsMCwxLDE5LjE1LDIuMDhMMzkuNDMsMjAuNDVBOCw4LDAsMCwxLDM2LjUsMzRaIi8+PC9nPjwvZz48L3N2Zz4="
              alt=""
            />
          </li>
        </ol>
        <ol
          class="bg-stars-box"
          style="
            translate: none;
            rotate: none;
            scale: none;
            transform: translate(0px, 0px);
          "
        >
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMTU3LjY2IiB2aWV3Qm94PSIwIDAgMTYzLjMyIDE1Ny42NiI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik04Ny4wOCw5MC43OGw0OCwxNi41NS00Ny41My0xOGE1LjM3LDUuMzcsMCwwLDEsMi43OS0yLjQxbDczLTI3LjYxTDkwLDg0LjYzYTUuMzEsNS4zMSwwLDAsMS00LjM4LS40MywzLjA3LDMuMDcsMCwwLDEsLjE3LS4zMWwyOC45My0zOS4zNUw4NC40Myw4My4xMmwtLjEyLjEyYTUuMzMsNS4zMywwLDAsMS0xLjUtMy42Mkw4MS42NiwwLDgwLjUsNzkuNjJBNS4zMiw1LjMyLDAsMCwxLDc5LDgzLjI0YS42OC42OCwwLDAsMS0uMTItLjEyTDQ4LjY1LDQ0LjU0LDc3LjU4LDgzLjg5YTMuMDcsMy4wNywwLDAsMSwuMTcuMzEsNS4zMiw1LjMyLDAsMCwxLTQuMzguNDNMMCw1OS4zMyw3Myw4Ni45NGE1LjM5LDUuMzksMCwwLDEsMi44LDIuNDFsLTQ3LjUzLDE4LDQ4LTE2LjU1aC4wNmE1LjM0LDUuMzQsMCwwLDEtLjg4LDQuNEwzMS4xOSwxNTUuMzJsNDYuMjMtNTlhNS4zMiw1LjMyLDAsMCwxLDMuNDktMmwuNzUsNTEuNzcuNzUtNTEuNzdhNS4zMiw1LjMyLDAsMCwxLDMuNDksMmw0Ni4yMyw1OUw4Ny45LDk1LjE3YTUuMzQsNS4zNCwwLDAsMS0uODgtNC40WiIvPjxwYXRoIGQ9Ik0zNC4xLDQyLjg1YTY3LjI2LDY3LjI2LDAsMSwwLDk1LjEyLDBBNjcuMjQsNjcuMjQsMCwwLDAsMzQuMSw0Mi44NVptOTQuMDUsOTQuMDVjLTI2LjI1LDI2LjI1LTY4LjM1LDI2LjcyLTk0LDFzLTI1LjIxLTY3Ljc4LDEtOTQsNjguMzYtMjYuNzIsOTQtMVMxNTQuNDEsMTEwLjY1LDEyOC4xNSwxMzYuOVoiLz48L2c+PC9nPjwvc3ZnPg=="
              alt=""
            />
          </li>
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjMxLjI1IiB2aWV3Qm94PSIwIDAgMTYzLjUyIDIzMS4yNSI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik05OC41MiwxMDkuN2M1LjIyLTE1Ljc5LDI1LjQ5LTM2LjIsNjUtNzUuODMtMzguNjYsMzguNTQtNTksNTguNzgtNzQuNjcsNjQuNi02LjkyLTE1LjE4LTctNDMuOTEtNy4wOS05OC40Ny0uMDksNTUuOS0uMTcsODQuNy03LjYyLDk5LjU3QzYzLjM4LDk2Ljg5LDUyLjczLDg2LjQzLDM2LDY5Ljg2LDUzLjEyLDg3LjE1LDYzLjc0LDk4LDY2LDEwOS4wOWMtOS40NSw2LjMtMjQuNjEsNi40MS00OC45Myw2LjU0LDIzLjUxLjExLDM4LjQ1LjIzLDQ4LDUuOTItNS4yMiwxNS43OS0yNS40OSwzNi4yLTY1LDc1Ljg0LDM4LjY2LTM4LjU0LDU5LTU4Ljc5LDc0LjY3LTY0LjYxLDYuOTIsMTUuMTgsNyw0My45MSw3LjA5LDk4LjQ3LjA5LTU1LjkuMTctODQuNyw3LjYyLTk5LjU3LDEwLjc2LDIuNjgsMjEuNDEsMTMuMTQsMzguMTQsMjkuNzEtMTcuMTItMTcuMjktMjcuNzQtMjguMDktMzAtMzkuMjMsOS40NS02LjMsMjQuNjEtNi40MSw0OC45My02LjUzQzEyMywxMTUuNTEsMTA4LDExNS4zOSw5OC41MiwxMDkuN1oiLz48L2c+PC9nPjwvc3ZnPg=="
              alt=""
            />
          </li>
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjE4LjU4IiB2aWV3Qm94PSIwIDAgMTIyLjM1IDIxOC41OCI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik0xMjIuMzUsMTA5LjI5Yy02MC44Ny4zLTYxLC41NS02MS4xOCwxMDkuMjlDNjEsMTA5Ljg0LDYwLjg3LDEwOS41OSwwLDEwOS4yOSw2MC44NywxMDksNjEsMTA4Ljc0LDYxLjE3LDAsNjEuMzQsMTA4Ljc0LDYxLjQ4LDEwOSwxMjIuMzUsMTA5LjI5Wk0xMDAuODQsMS4xNWMtLjA2LDM4LjIzLS4xMSwzOC4zMS0yMS41LDM4LjQyLDIxLjM5LjExLDIxLjQ0LjE5LDIxLjUsMzguNDIuMDYtMzguMjMuMTEtMzguMzEsMjEuNTEtMzguNDJDMTAxLDM5LjQ2LDEwMC45LDM5LjM4LDEwMC44NCwxLjE1WiIvPjwvZz48L2c+PC9zdmc+"
              alt=""
            />
          </li>
        </ol>
        <ol class="coins-box">
          <li>
            <img
              src="../assets/coin_doge.a40268b.svg"
              alt=""
              class="coin coin-left"
            />
          </li>
          <li>
            <img
              src="../assets/coin_xpt_1.ea0ea9d.svg"
              alt=""
              class="coin coin-left"
            />
          </li>
          <li>
            <img
              src="../assets/coin_eth.5457aa2.svg"
              alt=""
              class="coin coin-left"
            />
          </li>
          <li>
            <img
              src="../assets/coin_dash.19be76b.svg"
              alt=""
              class="coin coin-left"
            />
          </li>
          <li>
            <img
              src="../assets/coin_usdt.e6f3bfd.svg"
              alt=""
              class="coin coin-left"
            />
          </li>
          <li>
            <img
              src="../assets/coin_dai_1.6c7b9a2.svg"
              alt=""
              class="coin coin-right"
            />
          </li>
          <li>
            <img
              src="../assets/coin_dash.19be76b.svg"
              alt=""
              class="coin coin-right"
            />
          </li>
          <li>
            <img
              src="../assets/coin_xpt_2.863a89e.svg"
              alt=""
              class="coin coin-right"
            />
          </li>
          <li>
            <img
              src="../assets/coin_xpt_3.9a77a8a.svg"
              alt=""
              class="coin coin-right"
            />
          </li>
          <li>
            <img
              src="../assets/coin_btc.4df9e28.svg"
              alt=""
              class="coin coin-right"
            />
          </li>
        </ol>
      </div>
      <div class="content pr">
        <h1 style="margin-top: 4.6875rem" class="text-main out-stroke-white">
          Unlock the Full Potential of Web5
        </h1>
        <h1 class="text-main text-main-2 out-stroke-white">
          Social, Play, Earn
        </h1>
        <h1 class="text-main out-stroke-white">Across Web2 &amp; Web3</h1>
        <p class="text-desc">Your Comprehensive Kit Box to Unlock Web5</p>
        <div class="btn-box">
          <a
            target="_blank"
            href="https://dapp.xplus.com/social/home?t=1700815114912"
            class="btn-base btn-hollow"
            >Launch Dapp</a
          >
          <a
            target="_blank"
            href="https://play.google.com/store/apps/details?id=com.xplus.wallet"
            class="btn-base btn-primary"
          >
            Download App
          </a>
        </div>
      </div>
    </div>
    <div class="ytwo section section-earning">
      <div class="wrapper container">
        <div class="earning-progress">
          <span class="progress-box"
            ><img
              src="../assets/earning_progress.98dc2eb.svg"
              alt=""
              class="progress-svg"
          /></span>
          <div class="earning-item">
            <i></i>
            <img
              src="../assets/earning_01.22ce476.png"
              alt=""
              class="progress-img"
            />
            <strong class="progress-title">Earn $XCOIN</strong>
            <p class="progress-desc">
              Earn $XCOIN with XPLUS app and boost earnings power through social
              engagement and missions.
            </p>
          </div>
          <div class="earning-item">
            <i></i>
            <img
              src="../assets/earning_02.ad50340.png"
              alt=""
              class="progress-img"
            />
            <strong class="progress-title">$XCOIN Calculations</strong>
            <p class="progress-desc">
              $XCOIN generation speed relies on earning power. Build Team,
              engage within X-social, and spread XPLUS to other social networks
              to boost your earning power and level up your account.
            </p>
          </div>
          <div class="earning-item">
            <i></i>
            <img
              src="../assets/earning_03.ecd81ea.png"
              alt=""
              class="progress-img"
            />
            <strong class="progress-title">Token Calculations</strong>
            <p class="progress-desc">
              Your account level, team members, $XCOIN amount, and social
              contributions determine your final $XPLUS token amount.
            </p>
          </div>
          <div class="earning-item">
            <i></i>
            <img
              src="../assets/earning_04.403f97a.png"
              alt=""
              class="progress-img"
            />
            <strong class="progress-title">Earn $XPLUS Token</strong>
            <p class="progress-desc">
              Claim your $XPLUS tokens based on XPLUS ecosystem calculations.
              $XPLUS plan to be listed in Q1 2024.
            </p>
          </div>
        </div>
      </div>
    </div>
    <div class="ythree">
      <div class="layer-bg">
        <ol
          class="bg-triangles-box"
          style="
            translate: none;
            rotate: none;
            scale: none;
            transform: translate(0%, 14.1966%) translate3d(0px, 0px, 0px);
          "
        >
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDIuMDYiIGhlaWdodD0iNDMuNzYiIHZpZXdCb3g9IjAgMCA0Mi4wNiA0Mi43NiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiA+PGRlZnM+PHN0eWxlPi5jbHMtMXtmaWxsOiM5YjliOWI7fTwvc3R5bGU+PC9kZWZzPjxnIGlkPSLlm77lsYJfMiIgZGF0YS1uYW1lPSLlm77lsYIgMiI+PGcgaWQ9ImJhY2tncm91bmQiPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTM2LjUsMzRsLTI2LDguMzdBOCw4LDAsMCwxLC4xOSwzMy4wNkw2LDYuMzJBOCw4LDAsMCwxLDE5LjE1LDIuMDhMMzkuNDMsMjAuNDVBOCw4LDAsMCwxLDM2LjUsMzRaIi8+PC9nPjwvZz48L3N2Zz4="
              alt=""
            />
          </li>
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDIuMDYiIGhlaWdodD0iNDMuNzYiIHZpZXdCb3g9IjAgMCA0Mi4wNiA0Mi43NiIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiA+PGRlZnM+PHN0eWxlPi5jbHMtMXtmaWxsOiM5YjliOWI7fTwvc3R5bGU+PC9kZWZzPjxnIGlkPSLlm77lsYJfMiIgZGF0YS1uYW1lPSLlm77lsYIgMiI+PGcgaWQ9ImJhY2tncm91bmQiPjxwYXRoIGNsYXNzPSJjbHMtMSIgZD0iTTM2LjUsMzRsLTI2LDguMzdBOCw4LDAsMCwxLC4xOSwzMy4wNkw2LDYuMzJBOCw4LDAsMCwxLDE5LjE1LDIuMDhMMzkuNDMsMjAuNDVBOCw4LDAsMCwxLDM2LjUsMzRaIi8+PC9nPjwvZz48L3N2Zz4="
              alt=""
            />
          </li>
        </ol>
        <ol
          class="bg-stars-box"
          style="
            translate: none;
            rotate: none;
            scale: none;
            transform: translate(0%, 23.661%) translate3d(0px, 0px, 0px);
          "
        >
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMTM3LjE3IiB2aWV3Qm94PSIwIDAgMTI4LjcyIDEzNy4xNyI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik02NC4zNiwwbC45MSw2Mi43NWE0LjI1LDQuMjUsMCwwLDAsNS42Myw0bDU3LjgyLTE5Ljk0TDcxLjIsNjguNTJBNC4yNSw0LjI1LDAsMCwwLDY5LjI4LDc1bDM0Ljg2LDQ3LjQxTDY3LjcsNzUuOTNhNC4yNSw0LjI1LDAsMCwwLTYuNjgsMEwyNC41OCwxMjIuNDIsNTkuNDQsNzVhNC4yNSw0LjI1LDAsMCwwLTEuOTItNi40OUwwLDQ2Ljc2LDU3LjgzLDY2LjdhNC4yNCw0LjI0LDAsMCwwLDUuNjItNFpNODMuNzEsNDUuMzlsMTguNzctMjUuNTRMODIuOTIsNDQuOEM4My4xOSw0NSw4My40NSw0NS4xOCw4My43MSw0NS4zOVptMTAsMzQuNzQtLjM1LDFMMTI2LDkyLjM2Wk00NS44LDQ0LjgsMjYuMjQsMTkuODUsNDUsNDUuMzlDNDUuMjcsNDUuMTgsNDUuNTQsNDUsNDUuOCw0NC44Wk0zNSw4MC4xMywyLjY5LDkyLjM2LDM1LjM2LDgxLjA5QzM1LjIzLDgwLjc3LDM1LjEyLDgwLjQ1LDM1LDgwLjEzWm0yOS4zNiwyMC44LS41MiwwLC41MiwzNi4yNi41My0zNi4yNloiLz48L2c+PC9nPjwvc3ZnPg=="
              alt=""
            />
          </li>
          <li>
            <img src="../assets/star_3.d46b29e.svg" alt="" />
          </li>
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjMxLjI1IiB2aWV3Qm94PSIwIDAgMTYzLjUyIDIzMS4yNSI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik05OC41MiwxMDkuN2M1LjIyLTE1Ljc5LDI1LjQ5LTM2LjIsNjUtNzUuODMtMzguNjYsMzguNTQtNTksNTguNzgtNzQuNjcsNjQuNi02LjkyLTE1LjE4LTctNDMuOTEtNy4wOS05OC40Ny0uMDksNTUuOS0uMTcsODQuNy03LjYyLDk5LjU3QzYzLjM4LDk2Ljg5LDUyLjczLDg2LjQzLDM2LDY5Ljg2LDUzLjEyLDg3LjE1LDYzLjc0LDk4LDY2LDEwOS4wOWMtOS40NSw2LjMtMjQuNjEsNi40MS00OC45Myw2LjU0LDIzLjUxLjExLDM4LjQ1LjIzLDQ4LDUuOTItNS4yMiwxNS43OS0yNS40OSwzNi4yLTY1LDc1Ljg0LDM4LjY2LTM4LjU0LDU5LTU4Ljc5LDc0LjY3LTY0LjYxLDYuOTIsMTUuMTgsNyw0My45MSw3LjA5LDk4LjQ3LjA5LTU1LjkuMTctODQuNyw3LjYyLTk5LjU3LDEwLjc2LDIuNjgsMjEuNDEsMTMuMTQsMzguMTQsMjkuNzEtMTcuMTItMTcuMjktMjcuNzQtMjguMDktMzAtMzkuMjMsOS40NS02LjMsMjQuNjEtNi40MSw0OC45My02LjUzQzEyMywxMTUuNTEsMTA4LDExNS4zOSw5OC41MiwxMDkuN1oiLz48L2c+PC9nPjwvc3ZnPg=="
              alt=""
            />
          </li>
        </ol>
        <ol class="coins-box">
          <li>
            <img
              src="../assets/coin_xpt_2.863a89e.svg"
              alt=""
              class="coin coin-right"
            />
          </li>
        </ol>
      </div>
      <div class="ythrcont">
        <h1 class="text-main">XPLUS Ecosystem - A Sharing Economy in Web3</h1>
        <p class="text-desc">Collaborate, Earn &amp; Share</p>
        <ul class="ecosystem-list flex">
          <li>
            <div class="item-box">
              <div class="item-intro">Social Economy</div>
              <div class="item-icon-box">
                <img
                  src="../assets/icon_xcommunity.7de39b5.png"
                  alt=""
                  class="item-icon"
                />
              </div>
              <p class="item-desc">Create Business With</p>
              <strong class="item-name">X-Social</strong>
              <a href="#Social" class="btn-base btn-active">Learn More</a>
            </div>
          </li>
          <li>
            <div class="item-box">
              <div class="item-intro">Growth Hacking</div>
              <div class="item-icon-box">
                <img
                  src="../assets/icon_fomo.7f81416.png"
                  alt=""
                  class="item-icon"
                />
              </div>
              <p class="item-desc">Acquire Web3 Users With</p>
              <strong class="item-name">X-FOMO</strong>
              <a href="#FOMO" class="btn-base btn-active">Learn More</a>
            </div>
          </li>
          <li>
            <div class="item-box">
              <div class="item-intro">Payment Tool</div>
              <div class="item-icon-box">
                <img
                  src="../assets/icon_xwallet.48f853a.png"
                  alt=""
                  class="item-icon"
                />
              </div>
              <p class="item-desc">Seamless Transfer With</p>
              <strong class="item-name">X-Wallet</strong>
              <a href="#Wallet" class="btn-base btn-active">Learn More</a>
            </div>
          </li>
        </ul>
      </div>
    </div>
    <div class="yfour" id="Social">
      <div class="content pr">
        <h1 class="text-main">X-Social</h1>
        <p class="text-desc">
          USERS Acquire Diverse On-chain Rewards <br />
          Unlock CREATOR Exclusive and High-Quality Content
        </p>
      </div>
      <div class="yfourbox">
        <div class="yfourlb flex">
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_01.91a72fc.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_02.c0497e5.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_03.789d937.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_04.12cb975.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_05.9aaf390.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_06.f04857a.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_01.91a72fc.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_02.c0497e5.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_03.789d937.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_04.12cb975.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_05.9aaf390.png" alt=""
          /></a>
          <a target="_blank" href="https://dapp.xplus.com/social/home">
            <img src="../assets/slide_06.f04857a.png" alt=""
          /></a>
        </div>
      </div>
    </div>
    <div class="yfive flex">
      <div class="yfiveleft">
        <h1 class="text-main">
          Connect, Create, Earn with Your Fans Take control of your earnings
        </h1>
        <ul class="intro-texts">
          <li @click="tabimg('0')" :class="activeimg == '0' ? 'activeli' : ''">
            Content Monetization on Web3
          </li>
          <li @click="tabimg('1')" :class="activeimg == '1' ? 'activeli' : ''">
            NFT Holder Membership System
          </li>
          <li @click="tabimg('2')" :class="activeimg == '2' ? 'activeli' : ''">
            Viral Acquisition Tools
          </li>
          <li @click="tabimg('3')" :class="activeimg == '3' ? 'activeli' : ''">
            Instant On-Chain Income
          </li>
          <li @click="tabimg('4')" :class="activeimg == '4' ? 'activeli' : ''">
            All-in-one X-Page
          </li>
        </ul>
      </div>
      <div class="yfiveright">
        <div :class="activeimg == '0' ? 'activebox' : ''">
          <img
            :class="activeimg == '0' ? 'activeshow' : ''"
            src="../assets/intro_01.5788e7d.png"
            alt=""
          />
        </div>
        <div :class="activeimg == '1' ? 'activebox' : ''">
          <img
            :class="activeimg == '1' ? 'activeshow' : ''"
            src="../assets/intro_02.36f572f.png"
            alt=""
          />
        </div>
        <div :class="activeimg == '2' ? 'activebox' : ''">
          <img
            :class="activeimg == '2' ? 'activeshow' : ''"
            src="../assets/intro_03.5d75ac3.png"
            alt=""
          />
        </div>
        <div :class="activeimg == '3' ? 'activebox' : ''">
          <img
            :class="activeimg == '3' ? 'activeshow' : ''"
            src="../assets/intro_04.96a50a7.png"
            alt=""
          />
        </div>
        <div :class="activeimg == '4' ? 'activebox' : ''">
          <img
            :class="activeimg == '4' ? 'activeshow' : ''"
            src="../assets/intro_05.e0e7619.png"
            alt=""
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
let activeimg = ref("0");
let headtab = ref("0");
let activetab = (str) => {
  headtab.value = str;
};
let tabimg = (str) => {
  activeimg.value = str;
};
</script>

<style scoped>
.yhead {
  width: 100%;
  position: fixed;
  left: 0;
  top: 0;
  z-index: 9;
  border-bottom: 0.25rem solid #000;
  color: #000;
  background: white;
}
.yheadbox {
  width: 59.078377%;
  margin: 0 auto;
  padding: 0.53125rem 0.625rem;
  box-sizing: border-box;
  align-items: center;
}
.yheadbleft {
  align-items: center;
}
.yheadbleft img {
  width: 5rem;
}
.yheadbltab {
  margin-left: 1.5625rem;
  align-items: center;
}
.yheadbltab > a {
  display: block;
  line-height: 2.375rem;
  font-size: 1rem;
  font-weight: 700;
  color: #000;
  opacity: 0.3;
  padding: 0 0.9375rem;
  box-sizing: border-box;
}
.yheadbltab > a:hover {
  border-radius: 10px;
  background-color: rgb(200, 200, 200);
}
.yheadbltab > .yheadtabactive {
  opacity: 1;
}
.yheadbright > a {
  line-height: 1;
  padding: 0.625rem;
  font-size: 1rem;
  font-weight: 700;
  border-radius: 0.625rem;
  color: rgba(0, 0, 0, 0.3);
  cursor: pointer;
  align-items: center;
  justify-content: center;
}
.yheadbright > a:hover {
  background-color: #efefef;
}
.yheadbrgj {
  align-items: center;
}
.yheadbrgj > span {
  display: block;
  width: 40px;
  height: 40px;
  margin: 0 5px;
  background-color: #999;
  -webkit-mask: url("data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAwCAMAAABg3Am1AAAAM1BMVEUAAAB3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3d3dXTyszAAAAEHRSTlMAwIBAEPCg0OBgIHCwMFCQGZriSwAAAc1JREFUSMe9VUeCwyAMpFcT8//XblSCSHAc+7Jz8QAaVMBCHcPZpi7C5aA7IW61/DLPW39HrO7MPPUV3nyTtDhZ7WkaPA7tDceAX6uKf34CR7itTlzAFW1RGCA+GKpC87F82mM4yT4pxFKUkKIxrHZgH8Dxgxywix1IRcWbD/Rbke5PRkk6CAWZ9UAlD9oiA8NAPE9DxmTVQLEpBhXEcHDTSh3OlO3IGVqMMIXKvGESIvaO1cTlNKxiQGHnXY3QrKa41WTkR9xj24YH9oI/HVQq6XUkEPh+Aw0iuoMqxZaKZTkgqYwcUeDjFIFVAyxgREyCS8d4LIKdKZccZVrmzIdgWYS5WwL7DwJ9T0BX76RKUlYypV+yXDuHhL9shkn7QoXKjxGshTHi9lD6HWR0dAMF+8pVYAoc024Y4M8cDvy4yJvUQi7vdD2nViHdpLcfXcOlqf+EqRFacidcbMSbw6eA+bSrkZ8x06MhF0IUEZMQKvbm8/UJjikXowxntSNd+n2EzNtYM5ym2zoluSq8cesLlJPYr29iqi6TC37rsl5fRcaDWyAGULnlwpzkuz6kgjhx3dQXWN1XxKxOUPbUZ/hg1S+0GjQElPRmDqz/ANfzPAbUol7wAAAAAElFTkSuQmCC")
    no-repeat center;
  -webkit-mask-size: 22px auto;
  cursor: pointer;
}
.yheadbrgj > span:hover {
  background: #000;
}
.yone {
  width: 100%;
  padding: 3.125rem 0 53.75rem;
  position: relative;
  overflow: hidden;
  background: #efefef;
}
.layer-bg {
  position: absolute;
  z-index: 0;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
}
.clips-box {
  position: absolute;
  z-index: 0;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
}
ol,
ul {
  margin: 0;
  padding: 0;
  list-style: none;
}
.item-phone {
  position: absolute;
  left: 50%;
  top: unset;
  bottom: 140px;
  margin-left: -140px;
  font-size: 0;
}
.clip-wrap {
  font-size: 0;
  overflow: hidden;
  background-image: url("../assets/icon_grid.94b9d73.png");
  background-size: auto 310px;
  background-color: #ffd35a;
  background-attachment: fixed;
}
.shape-stroke {
  stroke: #000;
  stroke-width: 8;
  fill: transparent;
}
.phone-hand {
  position: absolute;
  bottom: 4px;
  left: 3%;
  height: 180%;
}
.img-hand-beside {
  position: relative;
  z-index: 0;
  height: 100%;
}
.img-hand-phone {
  position: absolute;
  left: 17%;
  bottom: 0;
  z-index: 1;
  height: 100%;
}
.item-triangle {
  position: absolute;
  left: 50%;
  top: 0;
  margin: 46.52422% 0 0 -37.17%;
}
.bg-triangles-box {
  position: absolute;
  z-index: 1;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
}
.section .bg-triangles-box > li {
  position: absolute;
  left: 50%;
  top: 0;
  width: 0;
  height: 0;
}
.section-banner .bg-triangles-box > li:first-child {
  transform: translate3d(-31.016148%, 15.2619%, 0);
}
.section-banner .bg-triangles-box > li:first-child > img {
  transform: rotate(-50deg);
}
.section-banner .bg-triangles-box > li:nth-child(2) {
  transform: translate3d(-550px, 780px, 0);
}
.section-banner .bg-triangles-box > li:nth-child(2) > img {
  transform: rotate(30deg);
}
.section-banner .bg-triangles-box > li:nth-child(3) {
  transform: translate3d(40px, 50px, 0);
}
.section-banner .bg-triangles-box > li:nth-child(3) > img {
  transform: rotate(0deg);
}
.section-banner .bg-triangles-box > li:nth-child(4) {
  transform: translate3d(750px, 220px, 0);
}
.section-banner .bg-triangles-box > li:nth-child(4) > img {
  transform: rotate(30deg);
}
.bg-stars-box {
  position: absolute;
  z-index: 1;
  width: 100%;
  height: 100%;
  left: 0;
  top: 0;
}
.section .bg-stars-box > li {
  position: absolute;
  left: 50%;
  top: 0;
  width: 0;
  height: 0;
}
.section-banner .bg-stars-box > li:first-child {
  transform: translate3d(-816px, 610px, 0);
}
.section .bg-stars-box > li > img {
  transform: translate3d(-50%, -50%, 0);
}
.section-banner .bg-stars-box > li:nth-child(2) {
  transform: translate3d(-270px, 780px, 0);
}
.section .bg-stars-box > li > img {
  transform: translate3d(-50%, -50%, 0);
}
.section-banner .bg-stars-box > li:nth-child(3) {
  transform: translate3d(650px, 380px, 0);
}
.section .bg-stars-box > li > img {
  transform: translate3d(-50%, -50%, 0);
}
.coins-box {
  position: absolute;
  z-index: 2;
  width: 100%;
  height: 100%;
  left: 0;
  top: 3.8125rem;
}
.section .coins-box > li {
  animation-delay: 0.2s;
  margin: 0 0 0 -620px;
  position: absolute;
  left: 50%;
  top: 0;
  width: 0;
  height: 0;
  animation: yoyoCoin-data-v-122fdbcb 3s ease-in-out 0ms infinite;
}
@keyframes yoyoCoin-data-v-122fdbcb {
  0% {
    transform: translateZ(0);
  }
  50% {
    transform: translate3d(5px, 10px, 0);
  }
  100% {
    transform: translateZ(0);
  }
}
.section .coins-box .coin {
  width: 12.5rem;
  height: 12.5rem;
  object-fit: contain;
  transform: translate3d(-50%, -50%, 0);
}
.section-banner .coins-box > li:nth-of-type(2) {
  animation-delay: 0.4s;
  margin: 320px 0 0 -820px;
}
.section-banner .coins-box > li:nth-of-type(3) {
  -webkit-animation-delay: 0.6s;
  animation-delay: 0.6s;
  margin: 520px 0 0 -560px;
}
.section-banner .coins-box > li:nth-of-type(4) {
  -webkit-animation-delay: 0.8s;
  animation-delay: 0.8s;
  margin: 820px 0 0 -830px;
}
.section-banner .coins-box > li:nth-of-type(5) {
  -webkit-animation-delay: 1s;
  animation-delay: 1s;
  margin: 1040px 0 0 -280px;
}
.section-banner .coins-box > li:nth-of-type(6) {
  -webkit-animation-delay: 0.3s;
  animation-delay: 0.3s;
  margin: 0 0 0 300px;
}

.section-banner .coins-box > li:nth-of-type(7) {
  -webkit-animation-delay: 0.5s;
  animation-delay: 0.5s;
  margin: 30px 0 0 800px;
}
.section-banner .coins-box > li:nth-of-type(8) {
  -webkit-animation-delay: 0.7s;
  animation-delay: 0.7s;
  margin: 230px 0 0 520px;
}
.section-banner .coins-box > li:nth-of-type(9) {
  -webkit-animation-delay: 0.9s;
  animation-delay: 0.9s;
  margin: 520px 0 0 850px;
}
.section-banner .coins-box > li:nth-of-type(10) {
  margin: 970px 0 0 660px;
}
.section .content {
  position: relative;
  z-index: 1;
  max-width: 61.25rem;
  margin: 0 auto;
  padding: 0 0.625rem;
  box-sizing: content-box;
  text-align: center;
  overflow: visible;
}
.section-banner .text-main {
  font-family: "MarkerFeltWide";
  line-height: 1.4;
  font-size: 2.615rem;
  text-align: left;
  position: relative;
  white-space: normal;
  font-weight: 400;
}
.out-stroke-white {
  text-shadow: 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff, 0 0 6px #fff,
    0 0 6px #fff;
}
.text-desc {
  margin: 1em auto 0;
  font-weight: 700;
  font-size: 1.5rem;
  font-family: "ChalkboardSE";
}
.section-banner .text-desc {
  text-align: left;
}
.section-banner .btn-box {
  text-align: left;
  margin-top: 1.25rem;
  display: flex;
}
.section-banner .btn-box .btn-base {
  flex: 0 0 auto;
  width: 11.5625rem;
  margin-right: 1.875rem;
}
.btn-base {
  height: 2.7em;
  max-width: 340px;
  border-radius: 0.625rem;
  font-size: 1rem;
  font-weight: 700;
  white-space: nowrap;
  padding: 0 1em;
  font-family: "ChalkboardSE";
  display: flex;
  justify-content: center;
  align-items: center;
  border: 2px solid black;
  box-sizing: border-box;
}
.btn-base.btn-hollow {
  color: #ffd35a;
  border-color: #ffd35a;
  background-color: #000;
}
.btn-base.btn-hollow:hover {
  color: #000;
  border-color: #000;
  background-color: #ffd35a;
}
.btn-base.btn-primary {
  color: #000;
  border-color: #000;
  background-color: #ffd35a;
}
.btn-base.btn-primary:hover {
  color: #ffd35a;
  border-color: #ffd35a;
  background-color: #000;
}
.ytwo {
  padding: 3.125rem 0 6.15rem;
}
.wrapper {
  width: 100%;
  max-width: 59.07837%;
  min-width: 18.46199%;
  margin: -5rem auto 0;
  padding: 0 0.625rem;
}
.section-earning .earning-progress {
  position: relative;
  max-width: 60rem;
  margin: 0 auto;
  padding-top: 15rem;
  display: flex;
}
.section-earning .progress-box {
  position: absolute;
  right: 0;
  top: 15rem;
  width: 100%;
  padding: 0 10%;
  margin-top: -10%;
  box-sizing: border-box;
}
.section-earning .progress-svg {
  width: 100%;
}
.section-earning .earning-item {
  flex: 1 1 0;
  width: 0;
  position: relative;
  padding: 0 1.25rem;
}
.section-earning .earning-item:first-of-type {
  margin-top: 31.2%;
}
.section-earning .earning-item > i {
  position: absolute;
  left: 0;
  top: 0;
  width: 0.25rem;
  height: 4.5rem;
  background-color: black;
  border-radius: 0.25rem;
}
.section-earning .progress-img {
  position: absolute;
  left: 0;
  top: 0;
  display: block;
  width: 80%;
  margin-top: -60%;
  transform: translate3d(0, -50%, 0);
}
.section-earning .progress-title {
  display: block;
  font-size: 1.0625rem;
  font-weight: 700;
  color: black;
}
.section-earning .progress-desc {
  display: block;
  margin-top: 1.3em;
  font-size: 0.9375rem;
  color: black;
}
.section-earning .earning-item:nth-of-type(2) {
  margin-top: 20.8%;
}
.section-earning .earning-item:nth-of-type(3) {
  margin-top: 10.4%;
}
.section-earning .earning-item:nth-of-type(4) {
  margin-top: 0;
}
.ythree {
  width: 100%;
  padding: 4.375rem 0 6.25rem;
  position: relative;
}
.ythree .bg-triangles-box > li {
  position: absolute;
  left: 50%;
  top: 0;
  width: 0;
  height: 0;
}
.ythree .bg-triangles-box > li:first-child {
  transform: translate3d(-630px, 500px, 0);
}
.ythree .bg-triangles-box > li:first-child > img {
  transform: rotate(-50deg);
}
.ythree .bg-triangles-box > li:nth-child(2) {
  transform: translate3d(570px, 110px, 0);
}
.ythree .bg-triangles-box > li:nth-child(2) > img {
  transform: rotate(30deg);
}
.ythree .bg-stars-box > li {
  position: absolute;
  left: 50%;
  top: 0;
  width: 0;
  height: 0;
}
.ythree .bg-stars-box > li:first-child {
  transform: translate3d(-580px, 180px, 0);
}
.ythree .bg-stars-box > li:nth-child(2) {
  transform: translate3d(-840px, 450px, 0);
}
.ythree .bg-stars-box > li:nth-child(3) {
  transform: translate3d(750px, 500px, 0);
}
.ythree .bg-stars-box > li > img {
  transform: translate3d(-50%, -50%, 0);
}
.ythree .coins-box > li {
  position: absolute;
  left: 50%;
  top: 0;
  width: 0;
  height: 0;
  animation: yoyoCoin-data-v-122fdbcb 3s ease-in-out 0ms infinite;
  animation-delay: 0.2s;
  margin: 400px 0 0 630px;
}
@keyframes yoyoCoin-data-v-122fdbcb {
  0% {
    transform: translateZ(0);
  }
  50% {
    transform: translate3d(5px, 10px, 0);
  }
  100% {
    transform: translateZ(0);
  }
}
.ythree .coins-box .coin {
  width: 12.5rem;
  height: 12.5rem;
  object-fit: contain;
  transform: translate3d(-50%, -50%, 0);
}
.ythrcont {
  position: relative;
  z-index: 1;
  max-width: 59.078377%;
  margin: 0 auto;
  padding: 0 0.625rem;
  box-sizing: content-box;
  text-align: center;
  overflow: visible;
}
.ythree .text-main {
  width: 50%;
  line-height: 1.4;
  font-size: 2.625rem;
  font-weight: 400;
  font-family: "MarkerFeltWide";
  white-space: pre-wrap;
  text-align: center;
  margin: 0 auto;
}
.text-desc {
  font-size: 1.5rem;
}
.text-desc,
.text-sub {
  margin: 1em auto 0;
  font-weight: 700;
  text-align: center;
}
.ecosystem-list {
  margin: 6.25rem auto 0;
  display: flex;
  justify-content: space-between;
}
.ecosystem-list li {
  width: 32%;
}
.item-box {
  position: relative;
  padding: 1rem;
  border-radius: 0.5rem;
  border: 2px solid black;
  background-color: white;
  box-sizing: border-box;
}
.item-intro {
  height: 2.75rem;
  border-radius: 5px;
  font-size: 1.25rem;
  font-weight: 700;
  color: white;
  background-color: black;
  display: flex;
  align-items: center;
  justify-content: center;
}
.item-icon-box {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 6.25rem;
  margin: 0.625rem 0;
}
.item-icon-box > img {
  height: 3.75rem;
}
.ythree .ecosystem-list .item-desc {
  margin: 0.625rem auto;
  font-size: 1rem;
}
.ythree .ecosystem-list .item-name {
  display: block;
  margin: 0 auto;
  line-height: 1;
  font-size: 1.75rem;
  font-weight: 700;
  color: black;
}
.ythree .ecosystem-list .btn-base {
  margin-top: 1.875rem;
  width: 100%;
  height: 2.5rem;
  border-radius: 0.625rem;
  font-size: 1rem;
  font-weight: 700;
  white-space: nowrap;
  padding: 0 1em;
  border: 2px solid black;
}
.btn-base.btn-active {
  color: #000;
  border-color: #000;
  background-color: #ffd35a;
}
.yfour {
  padding: 4.375rem 0 6.25rem;
  position: relative;
}
.yfour .text-main {
  line-height: 1.4;
  font-size: 2.625rem;
  font-weight: 400;
  font-family: "MarkerFeltWide";
  white-space: pre-wrap;
  text-align: center;
  margin: 0 auto;
}
.yfourbox {
  width: 100%;
  margin-top: 3.75rem;
  overflow: hidden;
}
.yfourlb {
  width: 200%;
  align-items: center;
  justify-content: space-between;
  column-gap: 2rem;
  animation-duration: 15s;
  animation-name: lb;
  animation-iteration-count: infinite;
  animation-timing-function: linear;
}
@keyframes lb {
  0% {
    margin-left: 0%;
  }
  100% {
    margin-left: -100%;
  }
}
.yfourlb > a {
  width: 19.125rem;
  height: 43.75rem;
  display: inline-block;
}
.yfourlb > a > img {
  width: 100%;
}
.yfourlb > a:nth-child(2n) > img {
  margin-top: 5%;
}
.yfive {
  margin: 11.25rem auto 0;
  padding: 0 0.9375rem;
  width: 59.078377%;
  box-sizing: border-box;
}
.yfiveleft {
  flex: 1 1 0;
}
.yfiveleft .text-main {
  line-height: 1.4;
  font-size: 2.625rem;
  font-weight: 400;
  font-family: "MarkerFeltWide";
  white-space: pre-wrap;
  text-align: left;
  margin: 0 auto;
  box-sizing: border-box;
  padding-right: 1.875rem;
}
.yfiveright {
  width: 38%;
  flex: 0 0 auto;
  position: relative;
}
.yfiveright > div {
  position: absolute;
  width: 100%;
  visibility: hidden;
  z-index: 0;
}
.yfiveright > .activebox {
  visibility: initial;
  z-index: 2;
}
.yfiveright img {
  width: 100%;
  transition: all 0.3s;
  transform: scale(0.8);
  opacity: 0.6;
}
.yfiveright .activeshow {
  transition: all 0.5s;
  transform: scale(1);
  opacity: 1;
}
.intro-texts {
  width: 100%;
  padding-right: 1.875rem;
  box-sizing: border-box;
}
.intro-texts > li {
  width: 100%;
  margin: 1.875rem 0;
  padding: 0 1rem;
  height: 4.375rem;
  font-size: 1.875rem;
  color: #777;
  border-radius: 0.5rem;
  cursor: pointer;
  font-weight: 700;
  line-height: 4.375rem;
}
.intro-texts > .activeli {
  color: black;
  background: #ffd35a;
}
</style>
