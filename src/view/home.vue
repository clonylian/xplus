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
    <div class="ysix section section-xcommunity" id="Space">
      <div class="layer-bg">
        <ol class="clips-box">
          <li class="item-triangle">
            <div
              class="clip-wrap clip-triangle"
              style="clip-path: url('#clipXcommunityTriangle')"
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
                    id="shapeXcommunityTriangle"
                    transform="rotate(-30 180 180)"
                    d="M6.56,246.25,138.63,17.5a30,30,0,0,1,52,0L322.66,246.25a30,30,0,0,1-26,45H32.54A30,30,0,0,1,6.56,246.25Z"
                  ></path>
                  <clipPath id="clipXcommunityTriangle">
                    <use xlink:href="#shapeXcommunityTriangle"></use>
                  </clipPath>
                </defs>
                <use
                  xlink:href="#shapeXcommunityTriangle"
                  class="shape-stroke"
                ></use>
              </svg>
            </div>
          </li>
          <li class="item-circle">
            <div
              class="clip-wrap clip-circle"
              style="clip-path: url('#clipPathXcommunityCircle')"
            >
              <svg
                width="446"
                height="446"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <circle
                    id="shapeXcommunityCircle"
                    cx="223"
                    cy="223"
                    r="223"
                  ></circle>
                  <clipPath id="clipPathXcommunityCircle">
                    <use xlink:href="#shapeXcommunityCircle"></use>
                  </clipPath>
                </defs>
                <use
                  xlink:href="#shapeXcommunityCircle"
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
            transform: translate(0%, 7.9089%) translate3d(0px, 0px, 0px);
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
        </ol>
        <ol
          class="bg-stars-box"
          style="
            translate: none;
            rotate: none;
            scale: none;
            transform: translate(0%, 13.1814%) translate3d(0px, 0px, 0px);
          "
        >
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iOTUuNzQiIHZpZXdCb3g9IjAgMCA1My41OSA5NS43NCI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik01My41OSw0Ny44N2MtMjYuNjYuMTMtMjYuNzIuMjQtMjYuOCw0Ny44N0MyNi43Miw0OC4xMSwyNi42Niw0OCwwLDQ3Ljg3LDI2LjY2LDQ3Ljc0LDI2LjcyLDQ3LjYzLDI2Ljc5LDAsMjYuODcsNDcuNjMsMjYuOTMsNDcuNzQsNTMuNTksNDcuODdabS0zNS05LjI3YTEuMzMsMS4zMywwLDAsMS0yLjE5LDBDMTMuMjEsMzQsNy44OSwyOC40NS40MiwyMC43NWM3LjY5LDcuNDgsMTMuMjMsMTIuOCwxNy44NSwxNmExLjMzLDEuMzMsMCwwLDEsLjMzLDEuODRabTAsMTguNTdBMS4zMywxLjMzLDAsMCwxLDE4LjI3LDU5QzEzLjY1LDYyLjE5LDguMTEsNjcuNTEuNDIsNzVjNy40Ny03LjcsMTIuNzktMTMuMjMsMTYtMTcuODVhMS4zMywxLjMzLDAsMCwxLDIuMTksMFpNMzUsMzguNTdhMS4zMiwxLjMyLDAsMCwxLC4zMy0xLjg0YzQuNjItMy4xOCwxMC4xNS04LjUsMTcuODUtMTZDNDUuNywyOC40NSw0MC4zOCwzNCwzNy4yLDM4LjZhMS4zMywxLjMzLDAsMCwxLTIuMTksMFptMCwxOC41N2ExLjMzLDEuMzMsMCwwLDEsMi4xOSwwYzMuMTgsNC42Miw4LjUsMTAuMTUsMTYsMTcuODUtNy43LTcuNDgtMTMuMjMtMTIuOC0xNy44NS0xNkExLjMyLDEuMzIsMCwwLDEsMzUsNTcuMTdaIi8+PC9nPjwvZz48L3N2Zz4="
              alt=""
            />
          </li>
        </ol>
        <ol class="coins-box">
          <li>
            <img
              src="../assets/coin_dai_1.6c7b9a2.svg"
              alt=""
              class="coin coin-left"
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
        <h1 class="text-main">Grow With X-Social Economy</h1>
        <p class="text-desc">
          A Comprehensive Business Solutions in Web3 Space Built for Creators
        </p>
        <p class="text-thd">
          One-stop decentralized solutions with various tools to establish and
          grow your own business.
        </p>
        <div class="ecosystem-box">
          <div class="system-kernel">
            <img src="../assets/ecosystem_kernel.22cf5b1.svg" alt="" />
            <strong class="text-sub out-stroke-black"
              >Sustainable Sharing Economy</strong
            >
            <p class="pre-wrap">Communitynomics Automation for Your Business</p>
          </div>
          <ul class="system-list">
            <li style="top: 0%; left: 50%">
              <img src="../assets/ecosystem_economy.611caea.png" alt="" />
              <p style="bottom: 100%; left: 50%; transform: translateX(-50%)">
                Mirco-Economy Ecosystem
              </p>
            </li>
            <li style="top: 30%; left: 100%">
              <img src="../assets/ecosystem_nft.48b2574.png" alt="" />
              <p style="bottom: 100%; left: 30%">Asset-backed Equity NFTs</p>
            </li>
            <li style="top: 78%; left: 95%">
              <img src="../assets/ecosystem_distribution.4c9d9c3.png" alt="" />
              <p style="bottom: 100%; left: 70%">
                Co-Create Community with Profit Sharing Distribution
              </p>
            </li>
            <li style="top: 100%; left: 50%">
              <img src="../assets/ecosystem_token.2295c7f.png" alt="" />
              <p style="top: 100%; left: 50%; transform: translateX(-50%)">
                Issue Utility Tokens &amp; NFTs
              </p>
            </li>
            <li style="top: 78%; left: 8%">
              <img src="../assets/ecosystem_tool.c666dd4.png" alt="" />
              <p style="bottom: 100%; right: 90%">
                Customised Marketing &amp; Community Tools
              </p>
            </li>
            <li style="top: 30%; left: 0%">
              <img src="../assets/ecosystem_dao.7959b20.png" alt="" />
              <p style="bottom: 100%; right: 50%">
                Genuine Engagement with DAO
              </p>
            </li>
          </ul>
        </div>
        <p class="text-thd">
          Peer-to-peer-based collaborative model, profit sharing among NFT
          holders transparently and automatically.
        </p>
      </div>
    </div>
    <div class="yqi section section-fomo" id="FOMO">
      <div class="layer-bg">
        <ol class="clips-box">
          <li class="item-circle">
            <div
              class="clip-wrap clip-circle"
              style="clip-path: url('#clipPathFomoCircle')"
            >
              <svg
                width="266"
                height="266"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <circle
                    id="shapeFomoCircle"
                    cx="133"
                    cy="133"
                    r="133"
                  ></circle>
                  <clipPath id="clipPathFomoCircle">
                    <use xlink:href="#shapeFomoCircle"></use>
                  </clipPath>
                </defs>
                <use xlink:href="#shapeFomoCircle" class="shape-stroke"></use>
              </svg>
            </div>
          </li>
          <li class="item-square">
            <div
              class="clip-wrap clip-square"
              style="clip-path: url('#clipPathFomoSquare')"
            >
              <svg
                width="340"
                height="340"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <rect
                    id="shapeFomoSquare"
                    width="250"
                    height="250"
                    rx="20"
                    x="48"
                    y="50"
                    transform="rotate(30 170 170)"
                  ></rect>
                  <clipPath id="clipPathFomoSquare">
                    <use xlink:href="#shapeFomoSquare"></use>
                  </clipPath>
                </defs>
                <use xlink:href="#shapeFomoSquare" class="shape-stroke"></use>
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
            transform: translate(0%, 11.8156%) translate3d(0px, 0px, 0px);
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
            transform: translate(0%, 19.6927%) translate3d(0px, 0px, 0px);
          "
        >
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iOTUuNzQiIHZpZXdCb3g9IjAgMCA1My41OSA5NS43NCI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik01My41OSw0Ny44N2MtMjYuNjYuMTMtMjYuNzIuMjQtMjYuOCw0Ny44N0MyNi43Miw0OC4xMSwyNi42Niw0OCwwLDQ3Ljg3LDI2LjY2LDQ3Ljc0LDI2LjcyLDQ3LjYzLDI2Ljc5LDAsMjYuODcsNDcuNjMsMjYuOTMsNDcuNzQsNTMuNTksNDcuODdabS0zNS05LjI3YTEuMzMsMS4zMywwLDAsMS0yLjE5LDBDMTMuMjEsMzQsNy44OSwyOC40NS40MiwyMC43NWM3LjY5LDcuNDgsMTMuMjMsMTIuOCwxNy44NSwxNmExLjMzLDEuMzMsMCwwLDEsLjMzLDEuODRabTAsMTguNTdBMS4zMywxLjMzLDAsMCwxLDE4LjI3LDU5QzEzLjY1LDYyLjE5LDguMTEsNjcuNTEuNDIsNzVjNy40Ny03LjcsMTIuNzktMTMuMjMsMTYtMTcuODVhMS4zMywxLjMzLDAsMCwxLDIuMTksMFpNMzUsMzguNTdhMS4zMiwxLjMyLDAsMCwxLC4zMy0xLjg0YzQuNjItMy4xOCwxMC4xNS04LjUsMTcuODUtMTZDNDUuNywyOC40NSw0MC4zOCwzNCwzNy4yLDM4LjZhMS4zMywxLjMzLDAsMCwxLTIuMTksMFptMCwxOC41N2ExLjMzLDEuMzMsMCwwLDEsMi4xOSwwYzMuMTgsNC42Miw4LjUsMTAuMTUsMTYsMTcuODUtNy43LTcuNDgtMTMuMjMtMTIuOC0xNy44NS0xNkExLjMyLDEuMzIsMCwwLDEsMzUsNTcuMTdaIi8+PC9nPjwvZz48L3N2Zz4="
              alt=""
            />
          </li>
          <li>
            <img src="../assets/star_3.d46b29e.svg" alt="" />
          </li>
        </ol>
        <ol class="coins-box">
          <li>
            <img
              src="../assets/coin_btc.4df9e28.svg"
              alt=""
              class="coin coin-left"
            />
          </li>
        </ol>
      </div>
      <div class="content pr">
        <h1 class="text-main">X-FOMO</h1>
        <p class="text-desc">
          A Revolutionary Social Platform Designed to Explore communities, Earn
          Hot Project Tokens, and Unlock the Full Potential of Web3
        </p>
        <button type="button" class="btn-lanuch btn-base btn-active">
          Launch Dapp
        </button>
        <div class="scale-wrap-box">
          <div data-gsap="clip-fomo-1" class="scale-wrap scale-wrap-1">
            <div class="scale-content">
              <div class="clip-area"></div>
              <div class="clip-phone">
                <div class="phone-wrap">
                  <img
                    src="../assets/phone_fomo_1.f9b4a8d.png"
                    alt=""
                    class="img-phone"
                  />
                  <svg
                    viewBox="0 0 140 120"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                    class="tips-line"
                    style="top: 21%"
                  >
                    <defs>
                      <path
                        id="pathTipsLine0101"
                        fill="none"
                        stroke-linecap="round"
                        d="M 130,110 L 92,110 A 5,5 0,0,1 88,108 L 42,7 A 5,5 0,0,0 38,5 L 5,5"
                      ></path>
                    </defs>
                    <g>
                      <rect
                        x="120"
                        y="100"
                        width="20"
                        height="20"
                        rx="3"
                        fill="#ffffff"
                      ></rect>
                      <use
                        xlink:href="#pathTipsLine0101"
                        stroke-width="10"
                        stroke="#ffffff"
                        class="path-tips-line-1"
                      ></use>
                      <rect
                        x="122"
                        y="102"
                        width="16"
                        height="16"
                        rx="3"
                        fill="#000000"
                      ></rect>
                      <use
                        xlink:href="#pathTipsLine0101"
                        stroke-width="6"
                        stroke="#000000"
                        class="path-tips-line-1"
                      ></use>
                    </g>
                  </svg>
                  <svg
                    viewBox="0 0 140 120"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                    class="tips-line"
                    style="top: 38.4%"
                  >
                    <defs>
                      <path
                        id="pathTipsLine0102"
                        fill="none"
                        stroke-linecap="round"
                        d="M 130,110 L 92,110 A 5,5 0,0,1 88,108 L 42,7 A 5,5 0,0,0 38,5 L 5,5"
                      ></path>
                    </defs>
                    <g>
                      <rect
                        x="120"
                        y="100"
                        width="20"
                        height="20"
                        rx="3"
                        fill="#ffffff"
                      ></rect>
                      <use
                        xlink:href="#pathTipsLine0102"
                        stroke-width="10"
                        stroke="#ffffff"
                        class="path-tips-line-1"
                      ></use>
                      <rect
                        x="122"
                        y="102"
                        width="16"
                        height="16"
                        rx="3"
                        fill="#000000"
                      ></rect>
                      <use
                        xlink:href="#pathTipsLine0102"
                        stroke-width="6"
                        stroke="#000000"
                        class="path-tips-line-1"
                      ></use>
                    </g>
                  </svg>
                  <div class="tips-text out-stroke-black" style="top: 21%">
                    <span>Choose a fomo</span>
                  </div>
                  <div class="tips-text out-stroke-black" style="top: 38%">
                    <span>One-Click to Share &amp; Earn</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div data-gsap="clip-fomo-2" class="scale-wrap scale-wrap-2">
            <div class="scale-content">
              <div class="clip-area"></div>
              <div class="clip-phone">
                <div class="phone-wrap">
                  <img
                    src="../assets/phone_fomo_2.46f186f.png"
                    alt=""
                    class="img-phone"
                  />
                  <svg
                    viewBox="0 0 160 250"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                    class="tips-line"
                    style="top: 24.1%"
                  >
                    <defs>
                      <path
                        id="pathTipsLine0201"
                        fill="none"
                        stroke-linecap="round"
                        d="M 5,240 L 50,240 A 5,5 0,0,0 54,238 L 130,7 A 5,5 0,0,1 134,5 L 155,5"
                      ></path>
                    </defs>
                    <g>
                      <rect
                        x="0"
                        y="230"
                        width="20"
                        height="20"
                        rx="3"
                        fill="#ffffff"
                      ></rect>
                      <use
                        xlink:href="#pathTipsLine0201"
                        stroke-width="10"
                        stroke="#ffffff"
                        class="path-tips-line-2"
                      ></use>
                      <rect
                        x="2"
                        y="232"
                        width="16"
                        height="16"
                        rx="3"
                        fill="#000000"
                      ></rect>
                      <use
                        xlink:href="#pathTipsLine0201"
                        stroke-width="6"
                        stroke="#000000"
                        class="path-tips-line-2"
                      ></use>
                    </g>
                  </svg>
                  <svg
                    viewBox="0 0 160 250"
                    xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink"
                    class="tips-line"
                    style="top: 43%"
                  >
                    <defs>
                      <path
                        id="pathTipsLine0202"
                        fill="none"
                        stroke-linecap="round"
                        d="M 5,240 L 50,240 A 5,5 0,0,0 54,238 L 130,7 A 5,5 0,0,1 134,5 L 155,5"
                      ></path>
                    </defs>
                    <g>
                      <rect
                        x="0"
                        y="230"
                        width="20"
                        height="20"
                        rx="3"
                        fill="#ffffff"
                      ></rect>
                      <use
                        xlink:href="#pathTipsLine0202"
                        stroke-width="10"
                        stroke="#ffffff"
                        class="path-tips-line-2"
                      ></use>
                      <rect
                        x="2"
                        y="232"
                        width="16"
                        height="16"
                        rx="3"
                        fill="#000000"
                      ></rect>
                      <use
                        xlink:href="#pathTipsLine0202"
                        stroke-width="6"
                        stroke="#000000"
                        class="path-tips-line-2"
                      ></use>
                    </g>
                  </svg>
                  <div class="tips-text out-stroke-black" style="top: 24%">
                    <span>Instant Token Rewards</span>
                  </div>
                  <div class="tips-text out-stroke-black" style="top: 43%">
                    <span>Maximize Your Rewards by Inviting</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="yba section section-xwallet" id="Wallet">
      <div class="layer-bg">
        <ol class="clips-box">
          <li class="item-triangle">
            <div
              class="clip-wrap clip-triangle"
              style="clip-path: url('#clipXwalletTriangle')"
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
                    id="shapeXwalletTriangle"
                    transform="rotate(-15 180 180)"
                    d="M6.56,246.25,138.63,17.5a30,30,0,0,1,52,0L322.66,246.25a30,30,0,0,1-26,45H32.54A30,30,0,0,1,6.56,246.25Z"
                  ></path>
                  <clipPath id="clipXwalletTriangle">
                    <use xlink:href="#shapeXwalletTriangle"></use>
                  </clipPath>
                </defs>
                <use
                  xlink:href="#shapeXwalletTriangle"
                  class="shape-stroke"
                ></use>
              </svg>
            </div>
          </li>
          <li class="item-circle">
            <div
              class="clip-wrap clip-circle"
              style="clip-path: url('#clipPathXwalletCircle')"
            >
              <svg
                width="266"
                height="266"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <circle
                    id="shapeXwalletCircle"
                    cx="133"
                    cy="133"
                    r="133"
                  ></circle>
                  <clipPath id="clipPathXwalletCircle">
                    <use xlink:href="#shapeXwalletCircle"></use>
                  </clipPath>
                </defs>
                <use
                  xlink:href="#shapeXwalletCircle"
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
            transform: translate(0%, 8.7592%) translate3d(0px, 0px, 0px);
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
            transform: translate(0%, 14.5987%) translate3d(0px, 0px, 0px);
          "
        >
          <li>
            <img
              style="width: 462px; height: 444px"
              src="../assets/star_4.f96ab07.svg"
              alt=""
            />
          </li>
          <li>
            <img
              style="width: 112px; height: 200px"
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjE4LjU4IiB2aWV3Qm94PSIwIDAgMTIyLjM1IDIxOC41OCI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik0xMjIuMzUsMTA5LjI5Yy02MC44Ny4zLTYxLC41NS02MS4xOCwxMDkuMjlDNjEsMTA5Ljg0LDYwLjg3LDEwOS41OSwwLDEwOS4yOSw2MC44NywxMDksNjEsMTA4Ljc0LDYxLjE3LDAsNjEuMzQsMTA4Ljc0LDYxLjQ4LDEwOSwxMjIuMzUsMTA5LjI5Wk0xMDAuODQsMS4xNWMtLjA2LDM4LjIzLS4xMSwzOC4zMS0yMS41LDM4LjQyLDIxLjM5LjExLDIxLjQ0LjE5LDIxLjUsMzguNDIuMDYtMzguMjMuMTEtMzguMzEsMjEuNTEtMzguNDJDMTAxLDM5LjQ2LDEwMC45LDM5LjM4LDEwMC44NCwxLjE1WiIvPjwvZz48L2c+PC9zdmc+"
              alt=""
            />
          </li>
        </ol>
        <ol class="coins-box">
          <li>
            <img
              src="../assets/coin_xpt_2.863a89e.svg"
              alt=""
              class="coin coin-left"
            />
          </li>
        </ol>
      </div>
      <div class="content pr">
        <h1 class="text-main">X-Wallet</h1>
        <p class="text-sub out-stroke-black">
          The Seamless Portal to Connect Web3
        </p>
        <p class="text-desc">
          Manage any digital assets on all chains on one page, Discover Web3
          opportunities and use Dapp with instant rewards
        </p>
        <ul class="list-group">
          <li>
            <div class="item-box">
              <h2>Manage Assets with Social Connection</h2>
              <p>
                Freely transfer assets anytime with ease and connect with social
                chat using DID Technology. Multi-chain transactions are a snap
                with X-Wallet.
              </p>
              <div data-gsap="clip-wallet" class="clip-group-box">
                <div class="clip-area"></div>
                <div class="clip-phone">
                  <img
                    src="../assets/phone_wallet.994ae32.png"
                    alt=""
                    class="img-phone"
                    style="width: 100%; height: 100%"
                  />
                </div>
              </div>
            </div>
          </li>
          <li>
            <div class="item-box">
              <h2>X-Swap</h2>
              <p>
                Smartly match the best routes with the most liquidity and the
                best rates in a cross-chain environment. Securely swap
                multi-chain assets with an easy interface.
              </p>
              <div data-gsap="clip-swap" class="clip-group-box">
                <div class="clip-area"></div>
                <div class="clip-phone">
                  <img
                    src="../assets/phone_swap.9dcdbfc.png"
                    alt=""
                    class="img-phone"
                  />
                </div>
              </div>
            </div>
          </li>
        </ul>
      </div>
    </div>
    <div class="yjiu section section-roadmap">
      <div class="layer-bg">
        <ol class="clips-box">
          <li class="item-circle-1">
            <div
              class="clip-wrap clip-circle"
              style="clip-path: url('#clipPathRoadmapCircle')"
            >
              <svg
                width="266"
                height="266"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <circle
                    id="shapeRoadmapCircle"
                    cx="133"
                    cy="133"
                    r="133"
                  ></circle>
                  <clipPath id="clipPathRoadmapCircle">
                    <use xlink:href="#shapeRoadmapCircle"></use>
                  </clipPath>
                </defs>
                <use
                  xlink:href="#shapeRoadmapCircle"
                  class="shape-stroke"
                ></use>
              </svg>
            </div>
          </li>
          <li class="item-circle-2">
            <div
              class="clip-wrap clip-circle"
              style="clip-path: url('#clipPathRoadmapCircle2')"
            >
              <svg
                width="446"
                height="446"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <circle
                    id="shapeRoadmapCircle2"
                    cx="223"
                    cy="223"
                    r="223"
                  ></circle>
                  <clipPath id="clipPathRoadmapCircle2">
                    <use xlink:href="#shapeRoadmapCircle2"></use>
                  </clipPath>
                </defs>
                <use
                  xlink:href="#shapeRoadmapCircle2"
                  class="shape-stroke"
                ></use>
              </svg>
            </div>
          </li>
          <li class="item-pentagon">
            <div
              class="clip-wrap clip-pentagon"
              style="clip-path: url('#clipRoadmapPentagon')"
            >
              <svg
                width="190"
                height="190"
                xmlns="http://www.w3.org/2000/svg"
                xmlns:xlink="http://www.w3.org/1999/xlink"
                class="clip-svg"
              >
                <defs>
                  <path
                    id="shapeRoadmapPentagon"
                    d="M181.57,111.33l-56.88,72.43a20,20,0,0,1-22.62,6.43L15.61,158.47A20,20,0,0,1,2.51,139L6,46.92a20,20,0,0,1,14.52-18.5L109.07,3.26a20,20,0,0,1,22.08,8.1l51.3,76.48A20,20,0,0,1,181.57,111.33Z"
                  ></path>
                  <clipPath id="clipRoadmapPentagon">
                    <use xlink:href="#shapeRoadmapPentagon"></use>
                  </clipPath>
                </defs>
                <use
                  xlink:href="#shapeRoadmapPentagon"
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
            transform: translate(0%, 13.4757%) translate3d(0px, 0px, 0px);
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
            transform: translate(0%, 22.4595%) translate3d(0px, 0px, 0px);
          "
        >
          <li>
            <img
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIGhlaWdodD0iMjE4LjU4IiB2aWV3Qm94PSIwIDAgMTIyLjM1IDIxOC41OCI+PGcgaWQ9IuWbvuWxgl8yIiBkYXRhLW5hbWU9IuWbvuWxgiAyIj48ZyBpZD0i5Zu+5bGCXzYiIGRhdGEtbmFtZT0i5Zu+5bGCIDYiPjxwYXRoIGQ9Ik0xMjIuMzUsMTA5LjI5Yy02MC44Ny4zLTYxLC41NS02MS4xOCwxMDkuMjlDNjEsMTA5Ljg0LDYwLjg3LDEwOS41OSwwLDEwOS4yOSw2MC44NywxMDksNjEsMTA4Ljc0LDYxLjE3LDAsNjEuMzQsMTA4Ljc0LDYxLjQ4LDEwOSwxMjIuMzUsMTA5LjI5Wk0xMDAuODQsMS4xNWMtLjA2LDM4LjIzLS4xMSwzOC4zMS0yMS41LDM4LjQyLDIxLjM5LjExLDIxLjQ0LjE5LDIxLjUsMzguNDIuMDYtMzguMjMuMTEtMzguMzEsMjEuNTEtMzguNDJDMTAxLDM5LjQ2LDEwMC45LDM5LjM4LDEwMC44NCwxLjE1WiIvPjwvZz48L2c+PC9zdmc+"
              alt=""
            />
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
              src="../assets/coin_xpt_1.ea0ea9d.svg"
              alt=""
              class="coin coin-left"
            />
          </li>
          <li>
            <img
              src="../assets/coin_xpt_3.9a77a8a.svg"
              alt=""
              class="coin coin-right"
            />
          </li>
        </ol>
      </div>
      <div class="content pr">
        <h1 class="text-main">Roadmap</h1>
        <div class="timeline-box">
          <div class="timeline">
            <div class="timeline-item">
              <ul>
                <li class="group active">
                  <div class="box-title">
                    <span class="text-time"><strong>2023</strong></span>
                    <span class="check-wrap"><i class="check-box"></i></span>
                    <span class="text-title out-stroke-black">Q1</span>
                  </div>
                  <div class="text-content">
                    <p>XPLUS Dapp Beta</p>
                    <p>X-Wallet App</p>
                  </div>
                </li>
                <li class="group">
                  <div class="box-title">
                    <span class="text-time"><!----></span>
                    <span class="check-wrap"><i class="check-box"></i></span>
                    <span class="text-title out-stroke-black">Q2</span>
                  </div>
                  <div class="text-content">
                    <p>X-FOMO - Viral Referral System</p>
                    <p>X-FOMO - Instant Rewards Distribution</p>
                    <p>X-FOMO - On &amp; Off Chain Tasks</p>
                  </div>
                </li>
                <li class="group">
                  <div class="box-title">
                    <span class="text-time"><!----></span>
                    <span class="check-wrap"><i class="check-box"></i></span>
                    <span class="text-title out-stroke-black">Q3</span>
                  </div>
                  <div class="text-content">
                    <p>X-Social - Content Monetization</p>
                    <p>X-Page - All-in-one Social Page</p>
                    <p>X-Bonus - Social Mining</p>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
    <footer class="xfooter">
      <section class="section-connect">
        <div class="wrapper pr">
          <div class="links-title">Stay Connected With Us</div>
          <div class="box-social">
            <ul class="social-list">
              <li>
                <a
                  href="https://twitter.com/xplusio"
                  target="_blank"
                  aria-label="connect us on twitter"
                  class="social-app"
                  ><img
                    src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAAM1BMVEVMaXFPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT0/Gb0ahAAAAEHRSTlMAgKAwwGDQQBDw4JBQIHCwUKrDSwAAAAlwSFlzAAAWJQAAFiUBSVIk8AAAApJJREFUWIXtmcuS6yAMRMXLGD/5/6+dmjieOLYahA2re3ub5BQREmoEHWWUDfGuOu164uWG29S3gp4Z8vSY+9J4Xnevq3BjjIP5Bne1wDFG1wp8RFcGx+h38lgZHMN7G31tcIzrRq4di7jHY2oAjvaXvLYgx5mobwKOisi1IXcNUu4tItuIbJrkXHzlXSPwf/K/SrbKez+NqaZ8izz+9X7/V2fDuS4AOVU+3Vdzdi/rY6f+bIF48pCozO5kKMywLjNz/PDkETfdgXdY1/bBkz3u54YFm6sd5MnYNWneEcbYLafvYzKRYj7hHCGZxfeXDpIik7/8x45dMhuPJJn6844rMRiQP9vkv1uOA2CmmfLk5fCjL7YXg2GlHDV/zgewZm6vQXVP5zCqbeUgzgVkrtJmvygQjQIyqAgkzlmw5BAK0WLyQE5bW0DmOkC6UqTiGPCsKxF7aUDnc5EWOTmgCzQv1tuDrCtbNItA+VwSaf6ig8iB70qs+Cs79BtBvGpw0Uk4GS3cRu7QyHkkPUngwIJhslJqkUQE3c0SZFksLq4rTxZWC4hyMs6iw87An6d2UHJEY2eZzo0sOHEBTjvzLpMcqTt7zvNbxzq5XJCFt4kFgZOTzjw5nL2HDJwnw9Njysxm0+QwwijDChGQuxHFgajPT0U48uqU88l8WwRTat7JIJu8yYuGLcgxwvE3OeEQB3crzUV50uJpfTI3rPKf3DBeFQ2zBJVif1XClJLvyjecqrWaBPqG08t2E9e5DXkE15fnMplmdlubpajzYPWt7ahs8Oqxu6Bqr2G7wn7cVH9d+hyT0FDe07FxzK1e8Yj6au811wvONuB8LM6f9Op5YmvU8qfxQakPK27Le8O7oxOUiH4A09t1Rd892bAAAAAASUVORK5CYII="
                    alt=""
                /></a>
              </li>
              <li>
                <a
                  href="https://t.me/xplusofficial"
                  target="_blank"
                  aria-label="connect us on telegram"
                  class="social-app"
                  ><img
                    src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAAM1BMVEVMaXFPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT0/Gb0ahAAAAEHRSTlMA0GAwoPAQgEDA4JAgULBwv9EkeQAAAAlwSFlzAAAWJQAAFiUBSVIk8AAAApNJREFUWIXtmcmWhCAMRUEBh1LM/39tHwtRhgQRoVf1lt16DxXII4nM1bLpGUrFRacYro4XU63EiJDH99xdOlr3UIULAHL1uErXAgPA5oLrRMLqc5FFVTBAZ8FbZTBAb8CLrE7mbWIBNh5LAzDMrZYMsJ/q+lHeJRjrm4BBtjhyRj37NCKPbGpEHn7kH7kRWX5WIiHekfVKX84vyPOwHPVEXbJTs9Qkc6/O6mqR5af3iyB8Cx+TdcdC4cXKM/K5aZ7wZ5+QvUKzm20lhG9gPtnftH4CaaNNXEp55GDT1AAwn38his0c8hRs2jgD8OsXEF3CLTnaNLXXJw5YES/ekIVfZu87J00xcWotIPMt6gyW79MumGwWSLIUfYhlbJDmHVfUyghyuGlm50yyBf+iijeMjGeaOuwhAJPFW0yON+2r1RwuGcYINzqEzJHo7jt3pEMEpou3kIz1oIxtRzB5HCayKwvJAuH29hGO9NUUOI7zHMZZnQd2QsCE0RFnQ4r1YoynLWA/J1F9U5mijWmqq4lBwZTRpbObb0t3pQGWOrTRPXB+AkwZXb7z49lDG10uOc4Pq8RUJItMglMv55A5CU51qVn3IAlOdanvyKTRZZLxHGEpo8skDyQ5NX56QB5kZLHpt3LJIl49bXSZ5JGd8xXf+pNjhlyy9Twvz5PTnEyyw3DGfMm5bw5ZKW9x5yWcMLpM8hYcLnlYasLoinsroe7ypLgf3CNyM5os7jT152Ya95uc/Be53SSw3fQyaYXlki2nxA0n200G0N9pfJNzZ+ywwScEW1ZV+xp26m5EUayr2q78RcwtqqqinTv4/up5IBk1Hld79koTNg3o3rM13l0z1g9TuYvMesPW62gZSxR0zoyxP8+XlFNCSNthAAAAAElFTkSuQmCC"
                    alt=""
                /></a>
                <span class="social-name"><i>Announcement</i></span>
              </li>
              <li>
                <a
                  href="https://t.me/xplusio"
                  target="_blank"
                  aria-label="connect us on telegram"
                  class="social-app"
                  ><img
                    src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAAM1BMVEVMaXFPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT0/Gb0ahAAAAEHRSTlMA0GAwoPAQgEDA4JAgULBwv9EkeQAAAAlwSFlzAAAWJQAAFiUBSVIk8AAAApNJREFUWIXtmcmWhCAMRUEBh1LM/39tHwtRhgQRoVf1lt16DxXII4nM1bLpGUrFRacYro4XU63EiJDH99xdOlr3UIULAHL1uErXAgPA5oLrRMLqc5FFVTBAZ8FbZTBAb8CLrE7mbWIBNh5LAzDMrZYMsJ/q+lHeJRjrm4BBtjhyRj37NCKPbGpEHn7kH7kRWX5WIiHekfVKX84vyPOwHPVEXbJTs9Qkc6/O6mqR5af3iyB8Cx+TdcdC4cXKM/K5aZ7wZ5+QvUKzm20lhG9gPtnftH4CaaNNXEp55GDT1AAwn38his0c8hRs2jgD8OsXEF3CLTnaNLXXJw5YES/ekIVfZu87J00xcWotIPMt6gyW79MumGwWSLIUfYhlbJDmHVfUyghyuGlm50yyBf+iijeMjGeaOuwhAJPFW0yON+2r1RwuGcYINzqEzJHo7jt3pEMEpou3kIz1oIxtRzB5HCayKwvJAuH29hGO9NUUOI7zHMZZnQd2QsCE0RFnQ4r1YoynLWA/J1F9U5mijWmqq4lBwZTRpbObb0t3pQGWOrTRPXB+AkwZXb7z49lDG10uOc4Pq8RUJItMglMv55A5CU51qVn3IAlOdanvyKTRZZLxHGEpo8skDyQ5NX56QB5kZLHpt3LJIl49bXSZ5JGd8xXf+pNjhlyy9Twvz5PTnEyyw3DGfMm5bw5ZKW9x5yWcMLpM8hYcLnlYasLoinsroe7ypLgf3CNyM5os7jT152Ya95uc/Be53SSw3fQyaYXlki2nxA0n200G0N9pfJNzZ+ywwScEW1ZV+xp26m5EUayr2q78RcwtqqqinTv4/up5IBk1Hld79koTNg3o3rM13l0z1g9TuYvMesPW62gZSxR0zoyxP8+XlFNCSNthAAAAAElFTkSuQmCC"
                    alt=""
                /></a>
                <span class="social-name"><i>Group</i></span>
              </li>
              <li>
                <a
                  href="https://discord.com/invite/NcgfAn97Xv"
                  target="_blank"
                  aria-label="connect us on discord"
                  class="social-app"
                  ><img
                    src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAAM1BMVEVMaXFPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT0/Gb0ahAAAAEHRSTlMAIKCwEGDwwIBA4NAwUJBwvv0THQAAAAlwSFlzAAAWJQAAFiUBSVIk8AAAArFJREFUWIXtmUuWrCAMQFFEUPxk/6t9RyyRQGKDynkTMyutup0O+SNC6VRr4a6Mcm0ELUN7m3qIVQS5kY+5m9ghBs/9K2AAWDB4fYsLALoLwMuLYAB7otWrYAB5gKeXwQDrj3zfh1lpqtgCvD3GCmSn9FwDDK0Q4nlMU9ILIV4LPixDBZfbZRVDJfIiTCWy/sgf+T7ZLipOLWY2+ilZKld5cG4Z95rcXuaFS7JWR0FrALTW2kitdQ++qZgvstkFWU5Mx4O6KvbnPHnsMsAXSZgnJ70OpzVjbZYsM6C7MGWUJXNtJSG0A3Jkkw9mMjxD7jOPbxdSaYZcojKjNEMusLJglKbJbRmYdA+anOvLXog2iySPpWCq/ybJawYLC9G0kOTC8xOkOShyZIxGGRW592BMlAhTc1BkPBy59304502uk0dzDuHSFHlOwABntvfJzSIFssihMs3x8Ix3n5DRQSfBQpCRmc850SvtnyClE0MTZJSZz5H5SCWBRcMvJmFIkFE20sljhpwcIUFG4/75Tx5kb3k3MJznmkFGSePsYbwD+6DAeauU7KdQnVoUB0schQQZfV9Mu/cGQ/rhdtGSJHa7P8mia3sYDQo4ZQFknGnLybnykQvJRa1GETk89Eka9g8pjdJt3DhSGSlgbbs2GVcU4baGPc4wCYbKz32gS2c2XbSZz9rYDavcHrZBuWzSXobuN2RYY48UbbWT36eQSzK4jjEwL73LC+qDItdFbP/s2Q393tcqxWzOLiagfmkob/KvO7dWZtdb1/OgVB2/MJXXE+G3K/jI/4NcaxPYVttemoob14pb4nqb7TrbeNf01bhB+DWY1W49Kjier+pv3ocBarZf9jxb67LN4s5H1bp5JNucOzJSW5fhOXukbnid3qt8EJA6Xk3E0g13JNq2CCH+AdGcbqkMHDDUAAAAAElFTkSuQmCC"
                    alt=""
                /></a>
              </li>
            </ul>
            <ul class="social-list">
              <li>
                <a
                  href="https://medium.com/xpluscom"
                  target="_blank"
                  aria-label="connect us on medium"
                  class="social-app"
                  ><img
                    src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAAM1BMVEVMaXFPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT0/Gb0ahAAAAEHRSTlMA4KAgYBDwQIDAMNBQkLBwN/R7YgAAAAlwSFlzAAAWJQAAFiUBSVIk8AAAAmRJREFUWIXtmdGSgyAMRQMIoqDN/3/tjhY0ILRTCTP74H3bVU4jJCQEoNKDdHhXZrIzlKWkuY0NEkOBrJdW7C7hc/AsWMCIKHUCHri4iOh0J3CCHlnBBK2bfSLXEsgrNxhx7DIXm8ROnjqQcQsZ1QOMEwDYLmRUAPf3oI8aAPqAcYG5E3nq4nObXDcyPuSH/F/I0hItpZRj6BvFTa1MfiWJXRbesPSFIqP8X5PUUaUdXNHMX8yjlRU0STlyNXr9XlLUfMN9/lr/FVz3OknReaoU5yNdGf/Bn+ka+fqz6vj6E0GNzupJ1URG6h/pZNL1u0MeqdGJY3lOMg2zZJ5ukk84rSotgG8lT6dt5LChwdtWMpmRM8RXgLWdTOLlCHEPCtvJxHNjySO25WQgE6NDiNstbhjI5nKaUVusM5DpFrGHuNxPHxxkYvQe4n7f3TjIOCRGC4AXF5nEsg3rx0QmRmuD+j2Ah0xDXIaI4SHTEJ9DdmIiE6Pf68dGTooLwUomIR52Dy4yMVoyk2NX4UgtbWR1ko8Qjzm8iSxomRFJLvv7Fnmgw0Syfm1kmXx9CPEjYzWQY3RE1tvoozQgHl5rQlXIZ2MslqH++gVhhirorzW/dudHxF9Ju58VdJk8FgaOR8mRt1XL6CI5qcrDHoQylknXfm2xR/LDSTM6t5suaiT/qIf8kCtyHTuB/bqXHTuuPDc0F6nKdtKsCXp24zveIPQwOqQOxX5Tc6SOvOXSKpedmthkel22OVpuA4xsc72mN48AutSj/F2mdBOr2tnC5gZHu4e14Tp2Wi63uxl+vKPsqhsA/gDL9Je8nqatQAAAAABJRU5ErkJggg=="
                    alt=""
                /></a>
              </li>
              <li>
                <a
                  href="https://www.facebook.com/xpluscom"
                  target="_blank"
                  aria-label="connect us on facebook"
                  class="social-app"
                  ><img
                    src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAAM1BMVEVMaXFPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT0/Gb0ahAAAAEHRSTlMAoGAw8BAgQIDA4JCw0FBwClrI8QAAAAlwSFlzAAAWJQAAFiUBSVIk8AAAAblJREFUWIXt2duSgyAMBuCIKCrV8v5Pu+NpBJZIYnBvlv+28I1NKYwB/HSqmd3jjM0C6fTNc/WIbvrfdCd3twxdBLe6DOzc3AawKuWuJTEvwc6566lNWdjpk+6K1fjMfMiFVoWf4ZVabNnW9ecN2a5/vQfzpnHPhI7QAPDlqtZfr2DMkPQXbjHGgN0zpgZaAM6S08ndLCmPAAx4jnebG9lBK4Yxmb6aMVgutwgslgcMlsoaq4VYtigslRNHZxl5wmGh3MRcp9IgW/5GcItvc0w52oj6/G5DlaMfkHDAUeWoyJQZj+TlNXmocpWr/Afy4CWUjf8Rsk/fyUCLfU1+75mRQ6CAjM0Wyxggl7G3VLmMrW25jL2NyGWs1yKX0dlSGX2dFMvo/DvZeIke9PoA2TXqmVLlKle5yv9QJnbVHsjETuATmda9ZMsjtePKli21S8yWF2pnmyuvnW1aObjy1tEirWiuvHeHKA/NlI+3PMpNDU+eziYqoS3EkvXVUM7fiLFk5Q3N0gxZq2CsydSaLk9xbz1zW2qC3Iy1iQ64KXCBlbrhXdOrT7ZFi2dqFN6x38oSfnFqQgQAfgBw13iG3ITqTgAAAABJRU5ErkJggg=="
                    alt=""
                /></a>
              </li>
              <li>
                <a
                  href="https://www.instagram.com/xplus.app"
                  target="_blank"
                  aria-label="connect us on instagram"
                  class="social-app"
                  ><img
                    src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAAM1BMVEVMaXFPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT0/Gb0ahAAAAEHRSTlMAgDBg8KDgQMAQ0CBwULCQdMVQogAAAAlwSFlzAAAWJQAAFiUBSVIk8AAAAvFJREFUWIXNmeuyqyAMhbnITVF5/6c9IxG3QtJShJmz/rb9GkNYhMjuEtxOoVV2Xxku53Uz9dTEHYJeX3NDZOdct/XgHpqXB3iZe4FDmMQd3L5un9GuY8QRfSWkW46T5lQVvcEhnBXSpdyegnzI/uAQ1EHuvHygyTEmRoBDkIz5MWQ1oORAekhlRDH26dONG4P54iFj/PbJFARN1pKC/kla8ueGIk/+KxY2MJVNipy57AdRzk6QVS330P4DOYGdVJbU5tNz8WryaYJO4c95i+BkY1/EyKdxrzUHjYQYkGXEyFAVlRYIiTNVZA0R14FTHGVdI+T4Vfc9FVyYmF+BB4KQHbUmSABHVdgYdJHpkmzrQoacuSvoIpSSzOuWDyJl9C9K8kpsK634ajy/lspdNWHR6ijJBl1qZdJedhJSal1qgaYr+t/J88WN8nEVJqXO1Wgnq9yoxbMSmsmI8T07wVbyBrBltyHo7TxoHt1rI1lHlLuqZVqL3d9IlsXT77lTtJFhrz07NJ8VcBv5soe7lue/tZEXzEXU8++ayBq1yOmZjiayxZIB9uY6kLED4876H8lDsqFRV++xguOqDjb3kJ0yl6YJB9/t5tToSKZAg1/fmtt3Lnqd+hO0cvcTtdX5zyNF7Efc1oPzuw7OP/C0QtDZCKedHGbxAPusvl+QQ1B/bJk3h7WdTDxAkVZUK27MypHbpc3KmyJXdow37ejpQHW5v5Bjoooes70zf4ZS05lX3yaSRL4lSfKPNyAYc1XdgMbd2uJ06UDXJAQirr1ppjvI8nUZ7bl/am/Hf0ax+I2cuWnL040eTVyPKQQ+PaMmJ/b7pOcUNVGgpz2yDmx+nfbECdV37towoYpxb96Q8yRnpPo8VRs3CaSf55U0MV56LzVySjwm0dF7xk3jMaN6LSjWAUGn92L939Qk1+mdj9uLKzHqjVgxZOkHZsx12+RZd4k0mG0q35YeYfP3b3h3ynTXY1bUqllRb6Wv1TQtyiCMsX9234Wsc4wmBAAAAABJRU5ErkJggg=="
                    alt=""
                /></a>
              </li>
              <li>
                <a
                  href="https://www.youtube.com/channel/UCc7ruwFsOGrsQtHGWVs-O8g?sub_confirmation=1"
                  target="_blank"
                  aria-label="connect us on youtube"
                  class="social-app"
                  ><img
                    src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAFkAAABZCAMAAABi1XidAAAAM1BMVEVMaXFPT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT09PT0/Gb0ahAAAAEHRSTlMAIOBgEDDwQIDA0KBQkLBwAvxjkAAAAAlwSFlzAAAWJQAAFiUBSVIk8AAAAgFJREFUWIXtmduygyAMRfGG4DX//7VnqLa1ssEIZM6L+63tzBobQ7IT1FHdamtKlZ0nFVAzJFN36bEC6D79aY8y7Rk8F+ESUd39cNvsQHylGyEwER3QtiiY6BMQUxhMen+NXWkw0SgTC6f+lcgCYLKOvEiQqVKqFQHTqtQkQ7YCKbdLJjPodVqkyL3SYmQh8EN+yElkaxdjjOk3bW2i3T6s7gdjbcT4BMh67kN+56xuxe0ZkxfPjkQ1oXMMyfYWN9BJIRmZs7hAKUbk8TZYVTxyw0Cd5ecIIt8PBuofiJwABlYWkG9nhoKvkEu+SnDfAQDyAp/Jdujrj3yjBcgm8G/hDPKWf1ZukEn7M8hXWWSiOpzqmWQiG6qB2eRguAuQA+EuQcbhLkOmWYi8oEgXIA84O7LJOpTRueTwKcwjwwAXIAcCvIlV62B9NsEA55Kri9LPItdxBharpyR1WFYfpHhfwhpZZLYNPYjnZEC9uRLTfSW8QqZjxGclJrbLdcuJW2C2M3ddg28bOz8vImRXL+1ojJncvAPS0H09vYag0EbgmWEf8n+Q5TZUcls1uU1gsUuJk8Q2roPYlthIbrYFt/FyNwgSD/2esIsnnv64wLLXVkcvJHcjVhb967Rb3NoTVHudfipzWzojC9/ks4Pblc5knJphbC5GjmpfC9/TCaKU+gOK1GYXSmJnIwAAAABJRU5ErkJggg=="
                    alt=""
                /></a>
              </li>
            </ul>
          </div>
        </div>
      </section>
      <div class="wrapper container foot">
        <div class="agreement">
          <a href="/TermsAndPrivacy/Privacy.html" target="_blank"
            >Privacy agreement</a
          >
          <a href="/TermsAndPrivacy/Terms.html" target="_blank"
            >User agreement</a
          >
        </div>
        <p class="copyright">
          Copyrigt © 2021-2023 XPLUS Company. All rights reserved.
        </p>
      </div>
    </footer>
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
  padding: 3.125rem 0 53.75rem !important;
  position: relative;
  overflow: hidden;
  background: #efefef;
}
.section-banner .clips-box .item-phone {
  left: 50%;
  top: unset;
  bottom: 300px;
  margin-left: -140px;
  font-size: 0;
}
.section-banner .clips-box .phone-hand {
  position: absolute;
  bottom: 4px;
  left: 3%;
  height: 180%;
}
.section-banner .clips-box .img-hand-beside {
  position: relative;
  z-index: 0;
  height: 100%;
}
.section-banner .clips-box .img-hand-phone {
  position: absolute;
  left: 17%;
  bottom: 0;
  z-index: 1;
  height: 100%;
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
.section-fomo .clips-box .item-circle {
  left: 50%;
  margin: -95px 0 0 350px;
}
.section-fomo .clips-box .item-square {
  left: 50%;
  top: 430px;
  margin-left: -940px;
}
.section-fomo .bg-triangles-box > li:first-child {
  transform: translate3d(-530px, 300px, 0);
}
.section-fomo .bg-triangles-box > li:first-child > img {
  transform: rotate(30deg);
}
.section-fomo .bg-triangles-box > li:nth-child(2) {
  transform: translate3d(760px, 160px, 0);
}
.section-fomo .bg-triangles-box > li:nth-child(2) > img {
  transform: rotate(-40deg);
}
.section-fomo .bg-triangles-box > li:nth-child(3) {
  transform: translate3d(-750px, 950px, 0);
}
.section-fomo .bg-triangles-box > li:nth-child(3) > img {
  transform: rotate(0deg);
}
.section-fomo .bg-triangles-box > li:nth-child(4) {
  transform: translate3d(860px, 900px, 0);
}
.section-fomo .bg-triangles-box > li:nth-child(4) > img {
  transform: rotate(30deg);
}
.section-fomo .bg-stars-box > li:first-child {
  transform: translate3d(580px, 100px, 0);
}
.section-fomo .bg-stars-box > li:nth-child(2) {
  transform: translate3d(680px, 700px, 0);
}
.section-fomo .bg-stars-box > li:nth-child(2) > img {
  height: 200px;
}
.section-fomo .coins-box > li:first-of-type {
  -webkit-animation-delay: 0.4s;
  animation-delay: 0.4s;
  margin: 200px 0 0 -700px;
}
.section-fomo .coins-box > li:nth-of-type(2) {
  -webkit-animation-delay: 0.6s;
  animation-delay: 0.6s;
  margin: 700px 0 0 730px;
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
.section-xcommunity .clips-box .item-triangle {
  left: 50%;
  margin: 90px 0 0 580px;
}
.section .clips-box > li {
  position: absolute;
  left: 50%;
  top: 0;
}
.section-xcommunity .clips-box .item-circle {
  left: 50%;
  margin: 700px 0 0 -1000px;
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
.section-xcommunity .bg-triangles-box > li:first-child > img {
  transform: rotate(60deg);
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
.section-xcommunity .bg-triangles-box > li:nth-child(2) > img {
  transform: rotate(-40deg);
}
.section-xcommunity .bg-triangles-box > li:nth-child(3) > img {
  transform: rotate(30deg);
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
.section .bg-stars-box > li > img {
  transform: translate3d(-50%, -50%, 0);
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
.section-xcommunity .bg-stars-box > li:first-child {
  transform: translate3d(-700px, 280px, 0);
}
.section-xcommunity .bg-triangles-box > li:first-child {
  transform: translate3d(-530px, 250px, 0);
}
.section-xcommunity .bg-triangles-box > li:nth-child(2) {
  transform: translate3d(650px, 820px, 0);
}
.section-xcommunity .bg-triangles-box > li:nth-child(3) {
  transform: translate3d(-370px, 1000px, 0);
}
.section .coins-box > li {
  position: absolute;
  left: 50%;
  top: 0;
  width: 0;
  height: 0;
  -webkit-animation: yoyoCoin-data-v-122fdbcb 3s ease-in-out 0ms infinite;
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
.section-xcommunity .coins-box > li:first-of-type {
  -webkit-animation-delay: 0.8s;
  animation-delay: 0.8s;
  margin: 1300px 0 0 -650px;
}
.section-xcommunity .coins-box > li:nth-of-type(2) {
  -webkit-animation-delay: 0.6s;
  animation-delay: 0.6s;
  margin: 750px 0 0 780px;
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
  cursor: pointer;
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
  width: 7.53249%;
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
.ysix {
  padding: 4.375rem 0 6.25rem;
  position: relative;
}
.text-main {
  line-height: 1.4;
  font-size: 42px;
  font-family: "MarkerFeltWide";
  white-space: pre-wrap;
  text-align: center;
}
.text-desc,
.text-sub {
  margin: 1em auto 0;
  font-weight: 700;
  text-align: center;
}
.text-desc {
  font-size: 24px;
}
.section-xcommunity .text-desc {
  white-space: pre-wrap;
}
.section-xcommunity .text-thd {
  max-width: 520px;
  margin: 2.8em auto 0;
  font-size: 18px;
}
.section-xcommunity .ecosystem-box {
  position: relative;
}
.section-xcommunity .system-kernel {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate3d(-50%, -50%, 0);
}
.section-xcommunity .system-kernel > img {
  display: block;
  margin: 0 auto;
  height: 176px;
}
.section-xcommunity .system-kernel > strong {
  display: block;
  line-height: 1;
  margin-top: 30px;
  white-space: pre-wrap;
}
.section-xcommunity .text-sub {
  font-size: 36px;
}
.out-stroke-black {
  text-shadow: 0 0 2px #000, 0 0 2px #000, 0 0 2px #000, 0 0 2px #000,
    0 0 2px #000;
}
.text-desc,
.text-sub {
  margin: 1em auto 0;
  font-weight: 700;
  text-align: center;
}
.text-sub {
  color: #ffd35a;
}
.section-xcommunity .system-kernel > p {
  margin-top: 15px;
  font-size: 18px;
  white-space: pre-wrap;
}
.section-xcommunity .system-list {
  margin: 160px auto;
  width: 520px;
  height: 520px;
  position: relative;
  background: url("../assets/dashed_circle.6e8733a.svg") no-repeat;
  background-size: 100% 100%;
}
.section-xcommunity .system-list > li {
  width: 130px;
  height: 130px;
  position: absolute;
  transform: translate3d(-50%, -50%, 0);
}
.section-xcommunity .system-list > li > img {
  width: 100%;
  height: 100%;
}
.section-xcommunity .system-list > li > p {
  position: absolute;
  width: 180%;
  font-size: 18px;
}
.section-xcommunity .text-thd {
  max-width: 520px;
  margin: 2.8em auto 0;
  font-size: 18px;
}
.section {
  padding: 70px 0 100px;
  position: relative;
}
.section-fomo .clips-box .item-square {
  left: 50%;
  top: 430px;
  margin-left: -940px;
}
.section-fomo .text-desc {
  white-space: pre-line;
}
.section-fomo .btn-lanuch {
  margin-top: 50px;
  min-width: 220px;
  display: inline-block;
}
.btn-base.btn-active {
  color: #000;
  border-color: #000;
  background-color: #ffd35a;
}
.section-fomo .scale-wrap-box {
  position: relative;
  height: 600px;
  margin: 80px auto 20px;
  width: 93.88%;
}
.section-fomo .scale-wrap {
  width: 100%;
  height: 100%;
  margin: 0 auto;
  position: relative;
  overflow: visible;
}
.section-fomo .scale-wrap .scale-content {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
}
.section-fomo .clip-area {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 28.33%;
  border-radius: 180px;
  border: 4px solid #000;
  background-image: url("../assets/icon_grid.94b9d73.png");
  background-size: auto 310px;
  background-color: #ffd35a;
  background-attachment: fixed;
}
.section-fomo .clip-phone {
  position: absolute;
  top: 0;
  z-index: 1;
  bottom: 4px;
  width: 35.87%;
  overflow-y: clip;
}
.section-fomo .scale-wrap-1 .clip-phone {
  left: 18%;
}
.section-fomo .scale-wrap-2 {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
}
.section-fomo .scale-wrap {
  margin: 0 auto;
  overflow: visible;
}
.section-fomo .scale-wrap .scale-content {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
}
.section-fomo .clip-area {
  position: absolute;
  bottom: 0;
  left: 0;
  width: 100%;
  height: 28.33%;
  border-radius: 180px;
  border: 4px solid #000;
  background-image: url("../assets/icon_grid.94b9d73.png");
  background-size: auto 310px;
  background-color: #ffd35a;
  background-attachment: fixed;
}
.section-fomo .scale-wrap-2 .clip-area {
}
.section-fomo .clip-phone {
  position: absolute;
  top: 0;
  z-index: 1;
  bottom: 4px;
  width: 35.87%;
  overflow-y: clip;
}
.section-fomo .scale-wrap-2 .clip-phone {
  left: 48%;
}
.section-fomo .phone-wrap {
  position: absolute;
  /* top: 80%; */
  left: 0;
  width: 100%;
  transition: top 0.5s ease-out;
}
.section-fomo .scale-wrap-2 .phone-wrap {
  transform: translate3d(0, 9%, 0);
  transition-delay: 0.1s;
}
.section-fomo .img-phone {
  width: 100%;
}
.section-fomo .tips-line {
  position: absolute;
}
.section-fomo .tips-line {
  transition: visibility 0.8s linear;
}
.section-fomo .scale-wrap-2 .tips-line {
  position: absolute;
  left: 65%;
  width: 48.48%;
}
.section-fomo .tips-line {
}
.section-fomo .tips-line {
  transition: visibility 0.8s linear;
}
.section-fomo .scale-wrap-2 .tips-line {
  position: absolute;
  left: 65%;
  width: 48.48%;
}
.section-fomo .tips-text {
  margin-top: 5px;
  position: absolute;
  top: 0;
  line-height: 1.1;
  font-size: 18px;
  transform: translate3d(0, -50%, 0);
  font-weight: 700;
  color: #ffd35a;
  white-space: pre;
}
.section-fomo .scale-wrap-2 .tips-text {
  left: 115%;
  text-align: left;
}
.section-fomo .tips-text > span {
  display: inline-block;
}
.section-fomo .scale-wrap-2 .tips-text > span {
  transform-origin: 0 50%;
}
.section-fomo .scale-wrap-1 .tips-text {
  right: 115%;
  text-align: right;
}
.section-fomo .scale-wrap-1 .tips-text {
  right: 115%;
  text-align: right;
}
.section-fomo .scale-wrap-1 .tips-line {
  right: 70%;
  width: 42.42%;
}
.section-xwallet .clips-box .item-triangle {
  left: 50%;
  margin: 90px 0 0 490px;
}
.section-xwallet .clips-box .item-circle {
  left: 50%;
  margin: 1600px 0 0 -580px;
}
.section-xwallet .bg-triangles-box > li:first-child {
  transform: translate3d(750px, 700px, 0);
}
.section-xwallet .bg-triangles-box > li:first-child > img {
  transform: rotate(0deg);
}
.section-xwallet .bg-triangles-box > li:nth-child(2) > img {
  transform: rotate(30deg);
}
.section-xwallet .bg-stars-box > li:first-child {
  transform: translate3d(-700px, 110px, 0);
}
.section-xwallet .bg-stars-box > li:nth-child(2) {
  transform: translate3d(720px, 800px, 0);
}
.section-xwallet .bg-stars-box > li:nth-child(2) > img {
  height: 200px;
}
.section-xwallet .coins-box > li:first-of-type {
  -webkit-animation-delay: 0.2s;
  animation-delay: 0.2s;
  margin: 1080px 0 0 -830px;
}
.section-xwallet .text-desc {
  white-space: pre-wrap;
}
.section-xwallet .list-group > li {
  position: relative;
  margin: 180px auto 0;
  max-width: 850px;
}
.section-xwallet .list-group .item-box {
  position: relative;
  padding-bottom: 30%;
  text-align: left;
  border: none;
  background-color: transparent;
}
.section-xwallet .list-group .item-box > h2 {
  display: flex;
  align-items: center;
  justify-content: flex-start;
  padding: 0 15px 0 50%;
  height: 4.5em;
  font-size: 30px;
  font-weight: 700;
  white-space: pre-wrap;
  color: white;
  border-radius: 22px;
  background-color: black;
}
.section-xwallet .list-group .item-box > p {
  position: relative;
  z-index: 1;
  padding: 20px 30px 20px 50%;
  font-size: 18px;
  color: black;
}
.section-xwallet .list-group .clip-group-box {
  position: absolute;
  top: -60px;
  left: 0;
  width: 50%;
  height: 595px;
  overflow: visible;
}
.section-xwallet .list-group .clip-area {
  position: absolute;
  bottom: 0;
  left: 0;
  margin: 0 auto 0 -40%;
  width: 180%;
  height: 33.96%;
  border-radius: 180px;
  border: 4px solid black;
  background-image: url("../assets/icon_grid.94b9d73.png");
  background-size: auto 310px;
  background-color: #ffd35a;
  background-attachment: fixed;
}
.section-xwallet .list-group .clip-phone {
  position: absolute;
  left: 0;
  right: 0;
  top: -8px;
  bottom: 10px;
  width: 374px;
  height: 600px;
  overflow: hidden;
}
.section-xwallet .list-group .clip-phone > img {
  width: 374px !important;
  height: 721px !important;
}
.text-sub {
  font-size: 30px;
  color: #ffd35a;
}
.text-desc,
.text-sub {
  margin: 1em auto 0;
  font-weight: 700;
  text-align: center;
}
.text-desc {
  font-size: 24px;
}
.section-xwallet .list-group .img-phone {
  position: absolute;
  left: 50%;
  top: 10%;
  transform: translateX(-50%);
  width: 88%;
  transition: top 0.5s ease-out;
}
.section-xwallet .list-group > li {
  position: relative;
  margin: 180px auto 0;
  max-width: 850px;
}
.section-xwallet .list-group > li:nth-child(2n) .item-box {
  text-align: right;
}
.section-xwallet .list-group > li:nth-child(2n) .item-box > h2 {
  justify-content: flex-end;
  padding: 0 50% 0 15px;
}
.section-xwallet .list-group > li:nth-child(2n) .item-box > p {
  padding: 20px 50% 20px 30px;
}
.section-xwallet .list-group > li:nth-child(2n) .clip-group-box {
  left: unset;
  right: 0;
}
.section-xwallet .list-group .clip-group-box {
  position: absolute;
  top: -60px;
  left: 0;
  width: 50%;
  overflow: visible;
}
.section-xwallet .list-group > li:nth-child(2n) .clip-area {
  left: unset;
  right: 0;
  margin: 0 -40% 0 auto;
}
.section-roadmap .clips-box .item-circle-1 {
  left: 50%;
  margin: 320px 0 0 -450px;
}
.section .clips-box > li {
  position: absolute;
  top: 0;
}
.section-roadmap .clips-box .item-circle-2 {
  left: 50%;
  margin: 1280px 0 0 490px;
}
.section-roadmap .clips-box .item-pentagon {
  left: 50%;
  margin: 1100px 0 0 -900px;
}
.section-roadmap .bg-triangles-box > li:first-child {
  transform: translate3d(-860px, 300px, 0);
}
.section-roadmap .bg-triangles-box > li:nth-child(2) {
  transform: translate3d(460px, 700px, 0);
}
.section-roadmap .bg-triangles-box > li:first-child > img {
  transform: rotate(-40deg);
}
.section-roadmap .bg-triangles-box > li:nth-child(2) > img {
  transform: rotate(30deg);
}
.section-roadmap .bg-stars-box > li:first-child {
  transform: translate3d(-670px, 400px, 0);
}
.section-roadmap .bg-stars-box > li:nth-child(2) {
  transform: translate3d(420px, 300px, 0);
}
.section-roadmap .coins-box > li:first-of-type {
  -webkit-animation-delay: 0.7s;
  animation-delay: 0.7s;
  margin: 920px 0 0 -540px;
}
.section-roadmap .coins-box > li:nth-of-type(2) {
  -webkit-animation-delay: 0.3s;
  animation-delay: 0.3s;
  margin: 630px 0 0 800px;
}
.section-roadmap .timeline-box {
  max-width: 950px;
  margin: 100px auto;
  position: relative;
  z-index: 5;
}
.section-roadmap .timeline {
  position: relative;
  color: #fff;
}
.section-roadmap .timeline .timeline-item {
  position: relative;
  min-height: 30px;
  line-height: 30px;
  font-size: 0;
}
.section-roadmap .timeline .timeline-item .box-title {
  position: relative;
  display: flex;
  height: 30px;
  align-items: center;
}
.section-roadmap .timeline .timeline-item .text-time {
  flex: 1 1 0;
  width: 0;
  padding: 0 40px 0 0;
  text-align: right;
  position: relative;
}
.section-roadmap .timeline .timeline-item .text-time > strong {
  display: inline-block;
  width: 124px;
  height: 54px;
  border-radius: 54px;
  line-height: 54px;
  text-align: center;
  font-size: 36px;
  font-weight: 700;
  color: white;
  background-color: black;
}
.section-roadmap .timeline .timeline-item .check-wrap {
  flex: 0 0 auto;
  width: 0;
  position: relative;
}
.section-roadmap .timeline .timeline-item .check-box {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate3d(-50%, -50%, 0);
  width: 36px;
  height: 36px;
  border: 3px solid white;
  border-radius: 50%;
  background-color: black;
}
.section-roadmap .timeline .timeline-item .text-title {
  flex: 1 1 0;
  width: 0;
  padding: 0 0 0 40px;
  font-size: 34px;
  font-weight: 700;
  text-align: left;
  color: white;
  white-space: pre-wrap;
  opacity: 0.5;
}
.section-roadmap .timeline .timeline-item .group.active .text-title {
  opacity: 1;
  color: #ffd35a;
}
.section-roadmap .timeline .timeline-item .text-content {
  width: 50%;
  margin: 0 0 0 auto;
  padding: 5px 15px 60px 35px;
  text-align: left;
  position: relative;
}
.section-roadmap .timeline .timeline-item .text-content > p {
  margin-top: 0.8em;
  font-size: 18px;
  line-height: 1.2;
  color: black;
  opacity: 0.5;
}
.section-roadmap .timeline .timeline-item .group.active .text-content > p {
  opacity: 1;
}
.section-roadmap .timeline .timeline-item .box-title {
  position: relative;
  display: flex;
  height: 30px;
  align-items: center;
}
.section-roadmap .timeline .timeline-item .text-time {
  flex: 1 1 0;
  width: 0;
  padding: 0 40px 0 0;
  text-align: right;
  position: relative;
}
.section-roadmap .timeline .timeline-item .check-wrap {
  flex: 0 0 auto;
  width: 0;
  position: relative;
}
.section-roadmap .timeline .timeline-item .check-box {
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate3d(-50%, -50%, 0);
  width: 36px;
  height: 36px;
  border: 3px solid black;
  border-radius: 50%;
  background-color: white;
}
.section-roadmap .timeline .timeline-item .text-title {
  flex: 1 1 0;
  width: 0;
  padding: 0 0 0 40px;
  font-size: 34px;
  font-weight: 700;
  color: white;
  text-align: left;
  white-space: pre-wrap;
  opacity: 0.5;
}
.section-roadmap .timeline .timeline-item .text-content {
  width: 50%;
  margin: 0 0 0 auto;
  padding: 5px 15px 60px 35px;
  text-align: left;
  position: relative;
}
.section-roadmap .timeline .timeline-item .group.active .check-box:after {
  background-color: #ffd35a;
}
.section-roadmap .timeline .timeline-item .check-box:after {
  content: "";
  width: 20px;
  height: 20px;
  border: 1px solid black;
  border-radius: 50%;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate3d(-50%, -50%, 0);
}
.section-roadmap .timeline .timeline-item .text-content {
  width: 44.75%;
  margin: 0 0 0 auto;
  padding: 5px 15px 60px 35px;
  text-align: left;
  position: relative;
}
.section-roadmap .timeline .timeline-item .text-content:before {
  content: "";
  position: absolute;
  left: 0;
  top: 10px;
  bottom: 10px;
  width: 5px;
  background-color: black;
  border-radius: 5px;
  transform: translateX(-50%);
}
.xfooter {
  border-top: 4px solid black;
}
.foot,
.xfooter {
  background-color: white;
}
.section-connect {
  padding: 50px 0 40px;
}
.wrapper {
  width: 100%;
  max-width: 1200px;
  min-width: 375px;
  margin: 0 auto;
}

.links-title {
  text-align: center;
  font-size: 38px;
  font-family: "MarkerFeltWide";
  text-transform: uppercase;
}
.box-social {
  display: flex;
  justify-content: center;
}
.social-list {
  display: flex;
  align-items: center;
  margin-left: 30px;
  font-size: 0;
}
.social-list:first-child {
  margin-left: 0;
}
.social-list > li {
  width: 44px;
  height: 44px;
  margin-left: 30px;
  margin-top: 20px;
  opacity: 0.4;
  transition: opacity 0.3s linear;
  position: relative;
}
.social-list > li:hover {
  opacity: 1;
}
.yjiu {
  overflow: hidden;
}
.social-list .social-app {
  display: block;
  width: 100%;
  height: 100%;
  position: relative;
}
.social-list .social-app > img {
  width: 100%;
  height: 100%;
}
.social-list .social-name {
  position: absolute;
  top: 100%;
  left: 50%;
  transform: translateX(-50%);
  font-size: 20px;
  line-height: 20px;
  color: #4f4f4f;
}
.social-list .social-name > i {
  display: inline-block;
  transform: scale(0.5);
}
.foot {
  padding-top: 10px;
  padding-bottom: 40px;
}
.agreement {
  display: flex;
  align-items: center;
  justify-content: center;
  grid-gap: 40px;
  gap: 40px;
  text-decoration: underline;
  margin-bottom: 20px;
}
.agreement a {
  font-size: 14px;
  opacity: 0.3;
  color: #000;
  transform: all 0.3s linear;
}
.agreement a:hover {
  opacity: 1;
}
.copyright {
  font-size: 12px;
  opacity: 0.4;
}
.box-social > ul:nth-child(2) {
  margin: 0;
}
.copyright {
  text-align: center;
}
</style>
