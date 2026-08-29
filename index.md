---
layout: default
title: GenBasic
description: >-
  GenBasic USB Wi-Fi and Bluetooth adapters and UL-listed power supplies for
  Raspberry Pi, Libre Computer and other single-board computers.
---

<section class="hero">
  <div class="hero-grid">
    <div class="hero-inner">
      <p class="eyebrow">USB wireless &amp; power</p>
      <h1>Wireless and power for <span class="grad">single-board computers.</span></h1>
      <p class="lede">
        Two USB adapters and a power supply, for boards that have to stay up:
        fixed specifications, in-kernel Linux drivers, and a UL-listed supply
        that holds 5&nbsp;V under load.
      </p>
      <p class="hero-actions">
        <a class="cta" href="{{ '/products/' | relative_url }}">See the products</a>
      </p>
    </div>
    <div class="hero-art" aria-hidden="true">
      <img src="{{ '/assets/img/wifi5-bt-mini.jpg' | relative_url }}" alt=""
           width="1500" height="1437" decoding="async">
    </div>
  </div>

  <div class="hero-stats">
    <div><b>2.4 / 5</b><span>GHz, dual band</span></div>
    <div><b>433</b><span>Mbps, 802.11ac</span></div>
    <div><b>WPA3</b><span>SAE &middot; 802.1X</span></div>
    <div><b>15 W</b><span>UL Listed, 5 V 3 A</span></div>
  </div>
</section>

<section id="approach">
  <div class="sec-head">
    <h2>How these are built</h2>
    <p>Three things we hold fixed, and what each one means on the bench.</p>
  </div>

  <div class="grid three">

    <article class="pillar">
      <p class="pillar-n">01</p>
      <h3>Quality</h3>
      <p>
        The supply is <b>UL Listed</b> — certified against a file number, not
        a claim printed on a box. The adapters draw inside a USB 2.0 port's
        500 mA, so populating several on one hub does not pull the rail down.
      </p>
    </article>

    <article class="pillar">
      <p class="pillar-n">02</p>
      <h3>Testing</h3>
      <p>
        Adapters are tested against the supply that powers them, which is why
        the documentation names one rather than leaving it to chance. Both run
        on current Linux LTS kernels and official Libre Computer images.
      </p>
    </article>

    <article class="pillar">
      <p class="pillar-n">03</p>
      <h3>Availability</h3>
      <p>
        A model number fixes one radio specification, so a unit bought later
        is the unit you qualified. In-kernel drivers mean nothing to rebuild
        when the OS updates.
      </p>
    </article>

  </div>
</section>

<section id="adapters">
  <div class="sec-head">
    <h2>Wireless adapters</h2>
    <p>Both sit on the kernel's own mac80211 / cfg80211 stack, so in-kernel
       wireless management works normally — no vendor tool, no out-of-tree
       module to rebuild every kernel upgrade.</p>
  </div>

  <div class="grid two">

    <article class="card">
      <a class="card-link" href="{{ '/products/rf/2a4m1/' | relative_url }}">
        <div class="shot">
          <img src="{{ '/assets/img/wifi4-nano.jpg' | relative_url }}"
               alt="GenBasic RF 2A4M1 Wi-Fi 4 USB nano adapter"
               width="1500" height="1257" loading="lazy" decoding="async">
        </div>
        <p class="pn">RF 2A4M1</p>
        <h3 class="card-title">Wi-Fi 4 USB 2 Nano Wireless Adapter</h3>
      </a>
      <ul class="highlights compact">
        <li>2.4 GHz 802.11b/g/n, up to 150 Mbps</li>
        <li>19 × 14 × 5 mm nano housing</li>
        <li>No Bluetooth radio</li>
      </ul>
      <p class="card-actions">
        <a class="cta buy" href="https://www.amazon.com/dp/B0BNFKJPXS">Buy on Amazon</a>
        <a class="spec-link" href="{{ '/products/rf/2a4m1/' | relative_url }}">Full specifications &rarr;</a>
      </p>
    </article>

    <article class="card">
      <a class="card-link" href="{{ '/products/rf/2a5r1b4/' | relative_url }}">
        <div class="shot">
          <img src="{{ '/assets/img/wifi5-bt-mini.jpg' | relative_url }}"
               alt="GenBasic RF 2A5R1B4 Wi-Fi 5 Bluetooth USB mini adapter"
               width="1500" height="1437" loading="lazy" decoding="async">
        </div>
        <p class="pn">RF 2A5R1B4</p>
        <h3 class="card-title">Wi-Fi 5 + BT 4.2 USB 2 Wireless Adapter</h3>
      </a>
      <ul class="highlights compact">
        <li>2.4 + 5 GHz 802.11ac, up to 433 Mbps</li>
        <li>Bluetooth 4.2 dual-mode</li>
        <li>33 × 15 × 8 mm</li>
      </ul>
      <p class="card-actions">
        <a class="cta buy" href="https://www.amazon.com/dp/B0CGF9LVL9">Buy on Amazon</a>
        <a class="spec-link" href="{{ '/products/rf/2a5r1b4/' | relative_url }}">Full specifications &rarr;</a>
      </p>
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
    Rates are PHY rates and need an access point advertising the wider channel
    — 40 MHz for 150 Mbps, 80 MHz for 433 Mbps. On 20 MHz the Wi-Fi 4 adapter
    tops out at 72.2 Mbps. Real throughput tracks signal to noise and runs near
    75% of PHY rate in a quiet environment at 10 m.
  </p>
</section>

<section id="power">
  <div class="sec-head">
    <h2>Power</h2>
    <p>Most "flaky USB" on a single-board computer is a power problem wearing
       a disguise. This is the supply the adapters are tested against.</p>
  </div>

  <div class="grid two">
    <article class="card">
      <a class="card-link" href="{{ '/products/power/5v3a/' | relative_url }}">
        <div class="shot">
          <img src="{{ '/assets/img/power-supply.jpg' | relative_url }}"
               alt="GenBasic 5V 3A 15W USB Type-C power supply with inline switch"
               width="1500" height="1489" loading="lazy" decoding="async">
        </div>
        <p class="pn">5V 3A &middot; UL Listed</p>
        <h3 class="card-title">15W USB Type-C Power Supply with Switch</h3>
      </a>
      <ul class="highlights compact">
        <li>5 V 3 A · 15 W, UL Listed</li>
        <li>USB Type-C, MicroUSB adapter included</li>
        <li>Inline switch with status LED, 1.5 m cable</li>
      </ul>
      <p class="card-actions">
        <a class="cta buy" href="https://www.amazon.com/dp/B0C8V23K7Z">Buy on Amazon</a>
        <a class="spec-link" href="{{ '/products/power/5v3a/' | relative_url }}">Full specifications &rarr;</a>
      </p>
    </article>

    <div class="callout">
      <h3>Why it matters for a dongle</h3>
      <p>
        An adapter that drops off the USB bus, disappears after a few minutes
        or runs slow is usually being browned out rather than failing. USB 2.0
        budgets a port 500 mA, and both adapters are designed to stay inside
        that — but only if the board itself is being fed 5 V under load.
      </p>
      <p>
        If a board reboots at random or the adapter never enumerates, check
        the supply and the cable gauge before suspecting the radio.
      </p>
    </div>
  </div>
</section>

<section id="linux">
  <div class="split">
    <div>
      <h2>On Linux</h2>
      <p class="big">
        No installer, no vendor daemon, no module to rebuild after every
        kernel upgrade.
      </p>
      <p>
        Both adapters sit on the kernel's <code>mac80211</code> and
        <code>cfg80211</code> frameworks, so NetworkManager, <code>iw</code>,
        <code>wpa_supplicant</code> and everything else that speaks to
        in-kernel wireless treats them as ordinary devices. AP mode and
        monitor mode both work.
      </p>
      <p>
        WPA3 SAE is supported alongside 802.1X access control — worth having,
        since WPA2 passwords no longer survive a determined offline attack.
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
