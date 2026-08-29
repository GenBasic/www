---
layout: default
title: GenBasic
description: >-
  GenBasic USB Wi-Fi and Bluetooth adapters and UL-listed power supplies for
  Raspberry Pi, Libre Computer and other single-board computers.
---

<section class="hero">
  <div class="hero-inner">
    <p class="eyebrow">Wireless adapters &amp; power for SBCs</p>
    <h1>Plug it in.<br><span class="grad">It just comes up.</span></h1>
    <p class="lede">
      USB Wi-Fi and Bluetooth adapters that need no driver install on current
      Linux kernels — and the UL-listed power supply that keeps them, and the
      board they are plugged into, actually running.
    </p>
    <div class="hero-stats">
      <div><b>2.4&nbsp;/&nbsp;5</b><span>GHz bands</span></div>
      <div><b>433</b><span>Mbps, Wi-Fi 5</span></div>
      <div><b>WPA3</b><span>SAE compliant</span></div>
      <div><b>15 W</b><span>UL-listed supply</span></div>
    </div>
  </div>
</section>

<section id="adapters">
  <div class="sec-head">
    <h2>Wireless adapters</h2>
    <p>Both built on the kernel's own <code>mac80211</code> / <code>cfg80211</code>
       stack, so in-kernel wireless management works normally — no vendor tool,
       no out-of-tree module to rebuild every kernel upgrade.</p>
  </div>

  <div class="grid two">

    <article class="card">
      <div class="shot">
        <img src="{{ '/assets/img/wifi4-nano.jpg' | relative_url }}"
             alt="GenBasic RF 2A4M1 Wi-Fi 4 USB nano adapter, a small black USB plug marked 2A4M1 and GenBasic"
             width="1500" height="1257" loading="lazy" decoding="async">
      </div>
      <p class="pn">RF 2A4M1</p>
      <h3>Wi-Fi 4 USB 2 Nano<br>Wireless Adapter</h3>
      <dl class="spec">
        <div><dt>Band</dt><dd>2.4 GHz</dd></div>
        <div><dt>Standard</dt><dd>802.11b/g/n</dd></div>
        <div><dt>Rate</dt><dd>up to 150 Mbps <span class="dim">(40 MHz)</span></dd></div>
        <div><dt>Bluetooth</dt><dd class="none">&mdash;</dd></div>
        <div><dt>Antenna</dt><dd>1T1R, 2 dBi integrated</dd></div>
        <div><dt>Size</dt><dd>19 &times; 14 &times; 5 mm</dd></div>
        <div><dt>Bus</dt><dd>USB 2.0 Type-A</dd></div>
      </dl>
      <p class="card-note">
        Small enough to leave the neighbouring USB ports clear, and low-power
        enough to live inside a USB 2.0 port's 500 mA budget.
      </p>
      <p><a class="cta ghost small" href="https://www.amazon.com/dp/B0BNFKJPXS">View on Amazon</a></p>
    </article>

    <article class="card feature">
      <div class="shot">
        <img src="{{ '/assets/img/wifi5-bt-mini.jpg' | relative_url }}"
             alt="GenBasic RF 2A5R1B4 Wi-Fi 5 Bluetooth USB mini adapter, a black USB plug marked GenBasic"
             width="1500" height="1437" loading="lazy" decoding="async">
      </div>
      <p class="pn">RF 2A5R1B4</p>
      <h3>Wi-Fi 5 + BT 4.2 USB 2<br>Wireless Adapter</h3>
      <dl class="spec">
        <div><dt>Bands</dt><dd>2.4 + 5 GHz</dd></div>
        <div><dt>Standard</dt><dd>802.11ac/b/g/n</dd></div>
        <div><dt>Rate</dt><dd>up to 433 Mbps <span class="dim">(80 MHz)</span></dd></div>
        <div><dt>Bluetooth</dt><dd class="yes">4.2</dd></div>
        <div><dt>Antenna</dt><dd>1T1R, 2 dBi integrated</dd></div>
        <div><dt>Size</dt><dd>33 &times; 15 &times; 8 mm</dd></div>
        <div><dt>Bus</dt><dd>USB 2.0 Type-A</dd></div>
      </dl>
      <p class="card-note">
        Dual-band with Bluetooth on the same dongle. Plug and play on Linux
        6.2 and newer, and on official Libre Computer images.
      </p>
      <p><a class="cta ghost small" href="https://www.amazon.com/dp/B0CGF9LVL9">View on Amazon</a></p>
    </article>

  </div>

  <div class="table-wrap">
    <table>
      <thead>
        <tr>
          <th scope="col">Adapter</th>
          <th scope="col">Bands</th>
          <th scope="col">Standard</th>
          <th scope="col">Max rate</th>
          <th scope="col">Bluetooth</th>
          <th scope="col">Size</th>
        </tr>
      </thead>
      <tbody>
        <tr>
          <th scope="row"><span class="pn">RF 2A4M1</span></th>
          <td>2.4 GHz</td><td>802.11b/g/n</td><td>150 Mbps</td>
          <td class="none">&mdash;</td><td>19 &times; 14 &times; 5 mm</td>
        </tr>
        <tr>
          <th scope="row"><span class="pn">RF 2A5R1B4</span></th>
          <td>2.4 + 5 GHz</td><td>802.11ac/b/g/n</td><td>433 Mbps</td>
          <td class="yes">4.2</td><td>33 &times; 15 &times; 8 mm</td>
        </tr>
      </tbody>
    </table>
  </div>

  <p class="fineprint">
    Quoted rates are PHY rates and need an access point advertising the wider
    channel — 40 MHz for 150 Mbps, 80 MHz for 433 Mbps. On 20 MHz channels the
    Wi-Fi 4 adapter tops out at 72.2 Mbps. Real throughput depends on signal to
    noise and runs near 75% of PHY rate in a quiet environment at 10 m.
  </p>
</section>

<section id="power">
  <div class="sec-head">
    <h2>Power</h2>
    <p>Most "flaky USB" on a single-board computer is a power problem wearing a
       disguise. This is the supply we test the adapters against.</p>
  </div>

  <div class="grid two">
    <article class="card">
      <div class="shot">
        <img src="{{ '/assets/img/power-supply.jpg' | relative_url }}"
             alt="GenBasic 5V 3A 15W USB Type-C power supply with an inline switch with red button and status LED"
             width="1500" height="1489" loading="lazy" decoding="async">
      </div>
      <p class="pn">5V 3A &middot; UL Listed</p>
      <h3>15W USB Type-C Power Supply<br>with Switch &amp; MicroUSB Adapter</h3>
      <dl class="spec">
        <div><dt>Output</dt><dd>5 V &nbsp;3 A &nbsp;15 W</dd></div>
        <div><dt>Connector</dt><dd>USB Type-C</dd></div>
        <div><dt>Included</dt><dd>MicroUSB adapter</dd></div>
        <div><dt>Cable</dt><dd>1.5 m</dd></div>
        <div><dt>Switch</dt><dd>Inline, status LED</dd></div>
        <div><dt>Safety</dt><dd class="yes">UL Listed</dd></div>
        <div><dt>Plug</dt><dd>US</dd></div>
      </dl>
      <p class="card-note">
        Fits Raspberry Pi 3 and 4 and Libre Computer boards — Type-C natively,
        MicroUSB with the bundled adapter. The switch saves unplugging the
        cable every reboot.
      </p>
      <p>
        <a class="cta ghost small" href="https://www.amazon.com/dp/B0C8V23K7Z">Single</a>
        <a class="cta ghost small" href="https://www.amazon.com/dp/B0C8V2SP25">5-pack</a>
      </p>
    </article>

    <div class="callout">
      <h3>Why it matters for a dongle</h3>
      <p>
        A wireless adapter that drops off the USB bus, disappears after a few
        minutes, or shows poor throughput is usually being browned out rather
        than failing. USB 2.0 gives a port 500 mA, and both adapters above are
        designed to stay inside that — but only if the board itself is being
        fed 5 V under load.
      </p>
      <p>
        If a board reboots at random or the adapter never enumerates, check the
        supply and the cable gauge before suspecting the radio.
      </p>
    </div>
  </div>
</section>

<section id="linux">
  <div class="split">
    <div>
      <h2>On Linux</h2>
      <p class="big">
        No installer, no vendor daemon, no module to rebuild after every kernel
        upgrade.
      </p>
      <p>
        Both adapters sit on the kernel's <code>mac80211</code> and
        <code>cfg80211</code> frameworks, so NetworkManager, <code>iw</code>,
        <code>wpa_supplicant</code> and everything else that speaks to in-kernel
        wireless treats them as ordinary devices. AP mode and monitor mode both
        work.
      </p>
      <p>
        WPA3 SAE is supported, alongside 802.1X network access control — worth
        having, since WPA2 passwords no longer survive a determined offline
        attack.
      </p>
    </div>
    <div class="panel">
      <p class="panel-label">Stack</p>
      <p class="panel-value">mac80211 / cfg80211</p>
      <hr>
      <p class="panel-label">Security</p>
      <p class="panel-value">WPA3 SAE &middot; 802.1X</p>
      <hr>
      <p class="panel-label">Modes</p>
      <p class="panel-value">station &middot; AP &middot; monitor</p>
      <hr>
      <p class="panel-label">Also runs on</p>
      <p class="panel-value">Windows</p>
    </div>
  </div>
</section>
