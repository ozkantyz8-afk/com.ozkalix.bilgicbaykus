<title>Bilgiç Baykuş Privacy Policy</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Poppins:wght@500;600;700&family=IBM+Plex+Mono:wght@400;500&family=IBM+Plex+Sans:wght@400;500;600&display=swap">

<style>
  :root {
    --ground: #FFF8EA;
    --surface: #FFFFFF;
    --surface-alt: #FCF2DE;
    --ink: #2E2A4A;
    --ink-soft: #635D83;
    --rule: #E7DDC9;
    --rule-strong: #D6C8AC;
    --accent: #3D348B;
    --accent-soft: #EDE9FA;
    --warn: #B23E29;
    --sun: #FFC93C;

    --display: "Poppins", "Segoe UI", system-ui, sans-serif;
    --body: "IBM Plex Sans", "Segoe UI", system-ui, sans-serif;
    --mono: "IBM Plex Mono", ui-monospace, "Cascadia Mono", monospace;
  }

  @media (prefers-color-scheme: dark) {
    :root:not([data-theme="light"]) {
      --ground: #17152C;
      --surface: #201D3C;
      --surface-alt: #262247;
      --ink: #EDEAF8;
      --ink-soft: #A6A0C8;
      --rule: #332E56;
      --rule-strong: #443E6E;
      --accent: #A99BFF;
      --accent-soft: #2A2550;
      --warn: #FF8A75;
      --sun: #FFC93C;
    }
  }

  :root[data-theme="dark"] {
    --ground: #17152C;
    --surface: #201D3C;
    --surface-alt: #262247;
    --ink: #EDEAF8;
    --ink-soft: #A6A0C8;
    --rule: #332E56;
    --rule-strong: #443E6E;
    --accent: #A99BFF;
    --accent-soft: #2A2550;
    --warn: #FF8A75;
    --sun: #FFC93C;
  }

  * { box-sizing: border-box; }

  body {
    background: var(--ground);
    color: var(--ink);
    font-family: var(--body);
    font-size: 16px;
    line-height: 1.7;
    margin: 0;
    -webkit-font-smoothing: antialiased;
  }

  .page {
    max-width: 46rem;
    margin: 0 auto;
    padding: clamp(2rem, 6vw, 4.5rem) clamp(1.25rem, 5vw, 2rem) 5rem;
  }

  /* ---------- masthead ---------- */

  .masthead {
    display: flex;
    align-items: center;
    gap: 0.85rem;
    padding-bottom: 1.5rem;
    border-bottom: 1px solid var(--rule);
  }

  .mark { flex: none; }

  .wordmark {
    font-family: var(--display);
    font-weight: 600;
    font-size: 1.05rem;
    letter-spacing: 0.01em;
    line-height: 1.25;
  }

  .wordmark span {
    display: block;
    font-family: var(--mono);
    font-weight: 400;
    font-size: 0.72rem;
    letter-spacing: 0.12em;
    text-transform: uppercase;
    color: var(--ink-soft);
    margin-top: 0.15rem;
  }

  h1 {
    font-family: var(--display);
    font-weight: 700;
    font-size: clamp(2.1rem, 6vw, 3rem);
    line-height: 1.08;
    letter-spacing: -0.02em;
    text-wrap: balance;
    margin: 2.5rem 0 0.75rem;
  }

  .standfirst {
    font-size: 1.05rem;
    color: var(--ink-soft);
    max-width: 34rem;
    margin: 0 0 2.25rem;
  }

  /* ---------- fact grid ---------- */

  .facts {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(13rem, 1fr));
    gap: 1px;
    background: var(--rule);
    border: 1px solid var(--rule);
    border-radius: 10px;
    overflow: hidden;
    margin-bottom: 2.5rem;
  }

  .fact {
    background: var(--surface);
    padding: 0.95rem 1.1rem;
  }

  .fact dt {
    font-family: var(--mono);
    font-size: 0.68rem;
    letter-spacing: 0.11em;
    text-transform: uppercase;
    color: var(--ink-soft);
    margin-bottom: 0.3rem;
  }

  .fact dd {
    margin: 0;
    font-size: 0.92rem;
    font-weight: 500;
    word-break: break-word;
  }

  .fact dd.code { font-family: var(--mono); font-weight: 400; font-size: 0.86rem; }

  /* ---------- at a glance ---------- */

  .glance {
    background: var(--surface-alt);
    border: 1px solid var(--rule-strong);
    border-radius: 12px;
    padding: 1.5rem 1.6rem 1.35rem;
    margin-bottom: 3rem;
  }

  .glance h2 {
    font-family: var(--display);
    font-size: 0.78rem;
    font-weight: 600;
    letter-spacing: 0.13em;
    text-transform: uppercase;
    color: var(--accent);
    margin: 0 0 0.9rem;
  }

  .glance ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: grid;
    gap: 0.6rem;
  }

  .glance li {
    display: grid;
    grid-template-columns: 1.15rem 1fr;
    gap: 0.6rem;
    align-items: start;
    font-size: 0.95rem;
  }

  .glance li::before {
    content: "";
    width: 0.5rem;
    height: 0.5rem;
    margin-top: 0.55rem;
    border-radius: 2px;
    background: var(--sun);
  }

  /* ---------- contents ---------- */

  nav.toc {
    margin-bottom: 3.25rem;
    padding-bottom: 2rem;
    border-bottom: 1px solid var(--rule);
  }

  nav.toc h2 {
    font-family: var(--mono);
    font-size: 0.7rem;
    font-weight: 500;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: var(--ink-soft);
    margin: 0 0 0.9rem;
  }

  nav.toc ol {
    list-style: none;
    counter-reset: toc;
    margin: 0;
    padding: 0;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(15rem, 1fr));
    gap: 0.35rem 1.75rem;
  }

  nav.toc li { counter-increment: toc; }

  nav.toc a {
    display: grid;
    grid-template-columns: 1.8rem 1fr;
    color: var(--ink);
    text-decoration: none;
    font-size: 0.92rem;
    padding: 0.15rem 0;
    border-radius: 4px;
  }

  nav.toc a::before {
    content: counter(toc, decimal-leading-zero);
    font-family: var(--mono);
    font-size: 0.78rem;
    color: var(--ink-soft);
  }

  nav.toc a:hover { color: var(--accent); }
  nav.toc a:hover::before { color: var(--accent); }

  /* ---------- sections ---------- */

  section {
    display: grid;
    grid-template-columns: 3.25rem 1fr;
    margin-bottom: 2.75rem;
    scroll-margin-top: 1.5rem;
  }

  .num {
    font-family: var(--mono);
    font-size: 0.82rem;
    color: var(--accent);
    padding-top: 0.45rem;
  }

  section > div { min-width: 0; }

  h2.head {
    font-family: var(--display);
    font-weight: 600;
    font-size: 1.28rem;
    line-height: 1.3;
    letter-spacing: -0.01em;
    text-wrap: balance;
    margin: 0 0 0.75rem;
  }

  h3 {
    font-family: var(--display);
    font-weight: 600;
    font-size: 0.98rem;
    margin: 1.6rem 0 0.5rem;
  }

  p { margin: 0 0 1rem; }

  ul.plain {
    margin: 0 0 1rem;
    padding-left: 1.15rem;
  }

  ul.plain li { margin-bottom: 0.4rem; }

  code {
    font-family: var(--mono);
    font-size: 0.88em;
    background: var(--accent-soft);
    color: var(--accent);
    padding: 0.1em 0.38em;
    border-radius: 4px;
  }

  a { color: var(--accent); text-decoration-thickness: 1px; text-underline-offset: 2px; }

  a:focus-visible,
  nav.toc a:focus-visible {
    outline: 2px solid var(--accent);
    outline-offset: 3px;
  }

  strong { font-weight: 600; }

  .note {
    border-left: 3px solid var(--sun);
    background: var(--surface);
    padding: 0.9rem 1.1rem;
    border-radius: 0 8px 8px 0;
    font-size: 0.93rem;
    margin: 0 0 1rem;
  }

  /* ---------- table ---------- */

  .table-wrap {
    overflow-x: auto;
    border: 1px solid var(--rule);
    border-radius: 10px;
    margin-bottom: 1rem;
  }

  table {
    border-collapse: collapse;
    width: 100%;
    min-width: 34rem;
    font-size: 0.88rem;
  }

  th, td {
    text-align: left;
    padding: 0.7rem 0.9rem;
    border-bottom: 1px solid var(--rule);
    vertical-align: top;
  }

  th {
    font-family: var(--mono);
    font-weight: 500;
    font-size: 0.7rem;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--ink-soft);
    background: var(--surface-alt);
    white-space: nowrap;
  }

  tbody tr:last-child td { border-bottom: none; }

  td.no { color: var(--ink-soft); }

  /* ---------- footer ---------- */

  footer {
    border-top: 1px solid var(--rule);
    padding-top: 1.5rem;
    font-size: 0.85rem;
    color: var(--ink-soft);
    display: flex;
    flex-wrap: wrap;
    gap: 0.5rem 1.5rem;
    justify-content: space-between;
  }

  footer .mono { font-family: var(--mono); font-size: 0.78rem; }

  @media (max-width: 34rem) {
    section { grid-template-columns: 1fr; gap: 0.15rem; }
    .num { padding-top: 0; }
  }

  @media (prefers-reduced-motion: no-preference) {
    html { scroll-behavior: smooth; }
  }
</style>

<div class="page">

  <header class="masthead">
    <svg class="mark" width="44" height="44" viewBox="0 0 48 48" role="img" aria-label="Bilgiç Baykuş owl mascot">
      <circle cx="24" cy="26" r="17" fill="var(--sun)"/>
      <path d="M24 9c-9.4 0-17 7.6-17 17 0 9.4 7.6 17 17 17s17-7.6 17-17c0-9.4-7.6-17-17-17zm0 5c6.6 0 12 5.4 12 12s-5.4 12-12 12-12-5.4-12-12 5.4-12 12-12z" fill="#8B5E3C"/>
      <circle cx="24" cy="27" r="12" fill="#FDF6E9"/>
      <circle cx="19" cy="25" r="4.6" fill="#FFFFFF" stroke="#8B5E3C" stroke-width="1.1"/>
      <circle cx="29" cy="25" r="4.6" fill="#FFFFFF" stroke="#8B5E3C" stroke-width="1.1"/>
      <circle cx="19" cy="25" r="2.1" fill="#2B2118"/>
      <circle cx="29" cy="25" r="2.1" fill="#2B2118"/>
      <path d="M24 30l-2.4 3h4.8z" fill="#FFC93C"/>
      <path d="M10 13h28l-14-6z" fill="#3D348B"/>
      <rect x="17" y="12.5" width="14" height="3.4" rx="1" fill="#332B75"/>
    </svg>
    <div class="wordmark">
      Bilgiç Baykuş
      <span>Privacy Policy</span>
    </div>
  </header>

  <h1>Privacy Policy</h1>
  <p class="standfirst">How the Bilgiç Baykuş children's learning app handles information — written for the parents and guardians who install it.</p>

  <dl class="facts">
    <div class="fact">
      <dt>Application</dt>
      <dd>Bilgiç Baykuş</dd>
    </div>
    <div class="fact">
      <dt>Package ID</dt>
      <dd class="code">com.ozkalix.bilgicbaykus</dd>
    </div>
    <div class="fact">
      <dt>Developer</dt>
      <dd>ozkalix</dd>
    </div>
    <div class="fact">
      <dt>Contact</dt>
      <dd class="code"><a href="mailto:ozkantrkylmz30@gmail.com">ozkantrkylmz30@gmail.com</a></dd>
    </div>
    <div class="fact">
      <dt>Effective date</dt>
      <dd>31 August 2026</dd>
    </div>
    <div class="fact">
      <dt>Platform</dt>
      <dd>Android (Google Play)</dd>
    </div>
  </dl>

  <div class="glance">
    <h2>At a glance</h2>
    <ul>
      <li>There is no account, no sign-in, and no password. The app never asks a child for a name, an age, an email address, a photo, or any other personal detail.</li>
      <li>Learning progress — which questions were answered correctly, which need more practice, and which badges were earned — is saved only on the device itself and is never uploaded anywhere.</li>
      <li>The app shows advertisements supplied by Google AdMob. This is the one part of the app that connects to the internet, and Google receives limited device information in order to serve those ads.</li>
      <li>Ads are configured as child-directed and are limited to general-audience (G-rated) content, so advertising is non-personalized.</li>
      <li>Uninstalling the app erases everything the app has stored. Progress can also be cleared at any time from Settings.</li>
    </ul>
  </div>

  <nav class="toc" aria-label="Contents">
    <h2>Contents</h2>
    <ol>
      <li><a href="#s1">Who we are</a></li>
      <li><a href="#s2">What the app stores on the device</a></li>
      <li><a href="#s3">What we do not collect</a></li>
      <li><a href="#s4">Advertising</a></li>
      <li><a href="#s5">Spoken audio and text-to-speech</a></li>
      <li><a href="#s6">Permissions</a></li>
      <li><a href="#s7">Children's privacy</a></li>
      <li><a href="#s8">Data summary table</a></li>
      <li><a href="#s9">Retention and deletion</a></li>
      <li><a href="#s10">Security</a></li>
      <li><a href="#s11">International users</a></li>
      <li><a href="#s12">Changes and contact</a></li>
    </ol>
  </nav>

  <section id="s1">
    <div class="num">01</div>
    <div>
      <h2 class="head">Who we are</h2>
      <p>Bilgiç Baykuş ("the app") is an offline question-and-answer learning game for children aged roughly three to eight. It is published on Google Play under the package identifier <code>com.ozkalix.bilgicbaykus</code> by <strong>ozkalix</strong> ("we", "us").</p>
      <p>This policy explains what information the app stores, what leaves the device, and who else is involved. It applies to the Android application only.</p>
    </div>
  </section>

  <section id="s2">
    <div class="num">02</div>
    <div>
      <h2 class="head">What the app stores on the device</h2>
      <p>All of the app's content — every question, answer, illustration, and fact across all age groups and categories — is bundled inside the installed app. Nothing is downloaded, and no question content is sent anywhere.</p>
      <p>To keep track of a child's progress, the app saves a small amount of data in the device's own private app storage:</p>
      <ul class="plain">
        <li><strong>Mastered questions</strong> — identifiers of questions that have been answered correctly at least once, used to show progress and award badges.</li>
        <li><strong>Questions to practise again</strong> — identifiers of questions that were answered incorrectly, so the app can offer them again later.</li>
        <li><strong>Badges earned</strong> — which age group and category combinations have been completed.</li>
        <li><strong>Sound setting</strong> — whether spoken audio is switched on or off.</li>
        <li><strong>Interface language</strong> — the language chosen for the app's buttons and labels.</li>
      </ul>
      <p>These are plain numbers and labels. They contain no names, no contact details, and nothing that identifies a person. They stay in the app's private storage on the device, are not transmitted to us, and are not backed up to any server we control.</p>
    </div>
  </section>

  <section id="s3">
    <div class="num">03</div>
    <div>
      <h2 class="head">What we do not collect</h2>
      <p>We want to be explicit about this, because the app is used by young children. The app does <strong>not</strong>:</p>
      <ul class="plain">
        <li>Ask for or store a name, nickname, date of birth, email address, phone number, or postal address.</li>
        <li>Offer accounts, sign-in, registration, or profiles of any kind.</li>
        <li>Access the camera, microphone, photo library, contacts, calendar, call history, or SMS messages.</li>
        <li>Request or use precise device location.</li>
        <li>Include any analytics, crash-reporting, attribution, or social media software development kit.</li>
        <li>Contain in-app purchases, subscriptions, or any payment mechanism.</li>
        <li>Provide chat, messaging, user-generated content, or links to social networks.</li>
        <li>Sell or rent information about its users to anyone.</li>
      </ul>
      <p>We receive no data about individual children or devices, and we have no way to identify who is using the app.</p>
    </div>
  </section>

  <section id="s4">
    <div class="num">04</div>
    <div>
      <h2 class="head">Advertising</h2>
      <p>The app is free and is funded by advertising. Ads are supplied by <strong>Google AdMob</strong>, a service operated by Google LLC. This is the only feature that requires an internet connection; every other part of the app works fully offline.</p>

      <h3>Where ads appear</h3>
      <ul class="plain">
        <li>A banner across the bottom of the category selection screen.</li>
        <li>A banner across the bottom of the question screen.</li>
        <li>An in-feed advertisement placed between groups of category buttons.</li>
        <li>A full-screen advertisement shown when moving from one question to the next.</li>
      </ul>

      <h3>What Google may receive</h3>
      <p>To select and deliver an advertisement, and to measure whether it was shown, Google's advertising software may collect or receive information such as: a device advertising identifier, the IP address of the connection (from which an approximate, city-level region may be inferred), the device model and operating system version, the app's package identifier, and whether an ad was displayed, viewed, or tapped. This information is collected by Google, not by us — we never see it.</p>

      <h3>How ads are restricted</h3>
      <p>Because this app is made for children, we configure Google's advertising software with the strictest settings it offers:</p>
      <ul class="plain">
        <li>Every ad request is tagged for <strong>child-directed treatment</strong>. Google therefore serves non-personalized ads and does not use the advertising identifier for interest-based advertising or remarketing in this app.</li>
        <li>Ad content is limited to a maximum rating of <strong>G (general audiences)</strong>.</li>
      </ul>
      <p>These settings are applied by the app on every ad request. Google's own handling of the data it collects is governed by its policies rather than ours:</p>
      <ul class="plain">
        <li><a href="https://policies.google.com/privacy" target="_blank" rel="noopener noreferrer">Google Privacy Policy</a></li>
        <li><a href="https://policies.google.com/technologies/partner-sites" target="_blank" rel="noopener noreferrer">How Google uses information from sites or apps that use its services</a></li>
      </ul>

      <div class="note">If the device is offline, ads simply do not load and the app continues to work normally. No part of the learning experience depends on advertising being available.</div>
    </div>
  </section>

  <section id="s5">
    <div class="num">05</div>
    <div>
      <h2 class="head">Spoken audio and text-to-speech</h2>
      <p>The app reads questions and encouragement aloud using the <strong>text-to-speech engine already installed on the device</strong>. The app does not record audio and does not use the microphone.</p>
      <p>When speech is requested, the text to be spoken — question text and the short educational facts that accompany correct answers — is passed to that engine. Depending on the device and its settings, the engine may be provided by Google, by the device manufacturer, or by another application the device owner has installed, and some engines process text using an online service. That processing is governed by the policy of whoever supplies the engine.</p>
      <p>Spoken audio can be turned off entirely with the sound toggle in the app's header. When it is off, the app makes no text-to-speech requests at all.</p>
    </div>
  </section>

  <section id="s6">
    <div class="num">06</div>
    <div>
      <h2 class="head">Permissions</h2>
      <p>The app declares only two Android permissions, both of which exist solely to support advertising:</p>
      <ul class="plain">
        <li><code>android.permission.INTERNET</code> — allows the advertising software to request ads.</li>
        <li><code>android.permission.ACCESS_NETWORK_STATE</code> — allows the advertising software to check whether a connection is available before trying.</li>
      </ul>
      <p>No sensitive or runtime permissions are requested. The app never prompts for access to location, camera, microphone, storage, or contacts.</p>
    </div>
  </section>

  <section id="s7">
    <div class="num">07</div>
    <div>
      <h2 class="head">Children's privacy</h2>
      <p>Bilgiç Baykuş is designed for children and is distributed in line with the Google Play Families policy requirements.</p>
      <p>We do not knowingly collect personal information from children, and the app is built so that there is nothing personal to collect: there is no account, no free-text entry, no camera or microphone use, and no way for a child to send information out of the app. All advertising is delivered under child-directed treatment with G-rated content only, as described in section 04.</p>
      <p>We aim to meet the requirements of the United States Children's Online Privacy Protection Act (COPPA) and, for users in the European Economic Area and the United Kingdom, the provisions of the General Data Protection Regulation that concern children.</p>
      <p>If you are a parent or guardian and you believe that any personal information about your child has somehow been collected, please contact us at the address in section 12 and we will investigate and respond promptly.</p>
    </div>
  </section>

  <section id="s8">
    <div class="num">08</div>
    <div>
      <h2 class="head">Data summary table</h2>
      <p>A consolidated view of everything described above.</p>
      <div class="table-wrap">
        <table>
          <thead>
            <tr>
              <th scope="col">Data</th>
              <th scope="col">Handled by</th>
              <th scope="col">Purpose</th>
              <th scope="col">Leaves the device?</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>Question progress, badges, settings</td>
              <td>The app</td>
              <td>Show progress; repeat difficult questions</td>
              <td class="no">No</td>
            </tr>
            <tr>
              <td>Advertising identifier</td>
              <td>Google AdMob</td>
              <td>Ad delivery and fraud prevention</td>
              <td>Yes — to Google</td>
            </tr>
            <tr>
              <td>IP address, approximate region</td>
              <td>Google AdMob</td>
              <td>Serve region-appropriate ads</td>
              <td>Yes — to Google</td>
            </tr>
            <tr>
              <td>Device model, OS version, app ID</td>
              <td>Google AdMob</td>
              <td>Format ads correctly; measurement</td>
              <td>Yes — to Google</td>
            </tr>
            <tr>
              <td>Ad impressions and taps</td>
              <td>Google AdMob</td>
              <td>Reporting and payment to the developer</td>
              <td>Yes — to Google</td>
            </tr>
            <tr>
              <td>Question text sent to be spoken</td>
              <td>Device text-to-speech engine</td>
              <td>Read questions and facts aloud</td>
              <td>Depends on the engine installed</td>
            </tr>
            <tr>
              <td>Names, emails, photos, location, contacts</td>
              <td class="no">Not collected</td>
              <td class="no">—</td>
              <td class="no">Never</td>
            </tr>
          </tbody>
        </table>
      </div>
      <p>We, the developer, receive only aggregate advertising performance reports from Google — totals such as impressions and revenue. These reports contain no information about individual users.</p>
    </div>
  </section>

  <section id="s9">
    <div class="num">09</div>
    <div>
      <h2 class="head">Retention and deletion</h2>
      <p>Progress data is kept on the device for as long as the app remains installed, so that a child can pick up where they left off. It is removed in either of two ways:</p>
      <ul class="plain">
        <li><strong>Reset progress in the app.</strong> Open Settings from the gear icon and choose the reset option. All mastered questions, practice lists, and badges are cleared immediately.</li>
        <li><strong>Uninstall the app.</strong> Removing the app deletes its private storage and everything in it. This is permanent — there is no cloud copy to restore from.</li>
      </ul>
      <p>Because we hold no personal data about you or your child, there is nothing for us to delete on our side. Requests concerning data held by Google in connection with advertising should be directed to Google, or managed through the Android system settings for ads.</p>
    </div>
  </section>

  <section id="s10">
    <div class="num">10</div>
    <div>
      <h2 class="head">Security</h2>
      <p>Progress data is written to the app's private storage area, which the Android operating system isolates from other applications on the device. We operate no servers and hold no user databases, which removes an entire category of risk: there is no account to be breached and no stored personal information to expose.</p>
      <p>Data transmitted by Google's advertising software is protected in transit by that software and by Google's own infrastructure.</p>
    </div>
  </section>

  <section id="s11">
    <div class="num">11</div>
    <div>
      <h2 class="head">International users</h2>
      <p>The app can be installed anywhere Google Play is available. Since the app itself keeps all of its data on the device, no international transfer of data takes place on our part.</p>
      <p>Advertising data collected by Google may be processed on servers in other countries, including the United States, under the terms set out in Google's privacy policy.</p>
      <p>Where the General Data Protection Regulation applies, the limited processing carried out for advertising is described in Google's documentation for publishers; the app applies child-directed and non-personalized settings to every ad request as described in section 04.</p>
    </div>
  </section>

  <section id="s12">
    <div class="num">12</div>
    <div>
      <h2 class="head">Changes and contact</h2>
      <p>If this policy changes — for example because a feature is added or an advertising setting is altered — the revised version will be published at this address and the effective date at the top will be updated. Material changes will also be noted in the app's Google Play release notes. Continuing to use the app after a change means the updated policy applies.</p>
      <h3>Get in touch</h3>
      <p>Questions, concerns, or requests about this policy or about privacy in Bilgiç Baykuş can be sent to:</p>
      <ul class="plain">
        <li>Developer: <strong>ozkalix</strong></li>
        <li>Email: <a href="mailto:ozkantrkylmz30@gmail.com">ozkantrkylmz30@gmail.com</a></li>
        <li>Application: <code>com.ozkalix.bilgicbaykus</code></li>
      </ul>
      <p>We aim to reply to privacy enquiries within thirty days.</p>
    </div>
  </section>

  <footer>
    <div>© 2026 ozkalix — Bilgiç Baykuş</div>
    <div class="mono">Effective 31 August 2026 · v1.0</div>
  </footer>

</div>
