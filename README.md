<!DOCTYPE html>
<html lang="am">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="theme-color" content="#09251d">
<title>አለማየሁ እቁብ | Alemayehu Equb</title>

<style>
:root {
  --bg: #071a15;
  --panel: #0e2b22;
  --panel2: #12372b;
  --gold: #e9c46a;
  --gold2: #f5d98d;
  --text: #f5f7f3;
  --muted: #b7c9c0;
  --line: #285143;
}

* {
  box-sizing: border-box;
}

html {
  scroll-behavior: smooth;
}

body {
  margin: 0;
  background: radial-gradient(circle at top right, #164735 0, #071a15 40%);
  color: var(--text);
  font-family: system-ui, -apple-system, "Segoe UI", sans-serif;
  line-height: 1.6;
}

button, input, select, textarea {
  font: inherit;
}

button {
  cursor: pointer;
  border: 0;
}

.wrap {
  width: min(1120px, 92%);
  margin: auto;
}

.topbar {
  position: sticky;
  top: 0;
  z-index: 20;
  background: #071a15ed;
  backdrop-filter: blur(12px);
  border-bottom: 1px solid var(--line);
}

.nav {
  min-height: 70px;
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 18px;
}

.brand {
  display: flex;
  align-items: center;
  gap: 10px;
  font-weight: 800;
}

.logo {
  display: grid;
  place-items: center;
  width: 42px;
  height: 42px;
  border-radius: 13px;
  background: linear-gradient(145deg, var(--gold2), #b78a2b);
  color: #10251b;
  font-size: 1.3rem;
}

.navlinks {
  display: flex;
  gap: 8px;
  flex-wrap: wrap;
}

.navlinks a {
  color: var(--muted);
  text-decoration: none;
  padding: 8px 11px;
  border-radius: 10px;
}

.navlinks a:hover {
  color: var(--gold2);
  background: #ffffff0b;
}

.hero {
  padding: 76px 0 58px;
  display: grid;
  grid-template-columns: 1.25fr .75fr;
  gap: 35px;
  align-items: center;
}

.eyebrow {
  color: var(--gold);
  font-weight: 800;
}

.hero h1 {
  font-size: clamp(2.1rem, 5vw, 4.2rem);
  line-height: 1.16;
}

.hero h1 span {
  color: var(--gold);
}

.lead,
.muted {
  color: var(--muted);
}

.actions {
  display: flex;
  gap: 12px;
  flex-wrap: wrap;
  margin-top: 26px;
}

.btn {
  padding: 11px 17px;
  border-radius: 12px;
  font-weight: 750;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  text-decoration: none;
}

.btn-primary {
  background: var(--gold);
  color: #13271e;
}

.btn-primary:hover {
  background: var(--gold2);
}

.btn-ghost {
  border: 1px solid var(--line);
  background: #ffffff08;
  color: var(--text);
}

.hero-card,
.card {
  background: linear-gradient(160deg, #12382b, #0b241c);
  border: 1px solid var(--line);
  border-radius: 22px;
  padding: 24px;
  box-shadow: 0 20px 60px #0002;
}

.coin {
  width: 100px;
  height: 100px;
  margin: 4px auto 16px;
  display: grid;
  place-items: center;
  border-radius: 50%;
  border: 3px solid var(--gold);
  color: var(--gold);
  font-size: 3rem;
}

.hero-card {
  text-align: center;
}

.hero-card h3,
.card h3 {
  color: var(--gold2);
}

.stats {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 14px;
  margin: 10px 0 58px;
}

.stat {
  background: #ffffff08;
  border: 1px solid var(--line);
  border-radius: 16px;
  padding: 18px;
  text-align: center;
}

.stat strong {
  display: block;
  font-size: 1.55rem;
  color: var(--gold);
}

.section {
  padding: 34px 0 52px;
  scroll-margin-top: 85px;
}

.grid3 {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 16px;
}

.feature-icon {
  font-size: 1.8rem;
}

.notice-list {
  display: grid;
  gap: 12px;
}

.notice {
  border: 1px solid var(--line);
  border-radius: 14px;
  padding: 16px;
  background: #ffffff06;
}

.notice strong {
  color: var(--gold2);
}

.admin-layout {
  display: grid;
  grid-template-columns: .8fr 1.2fr;
  gap: 18px;
  align-items: start;
}

.field {
  display: grid;
  gap: 6px;
  margin: 12px 0;
}

.field input,
.field select,
.field textarea {
  width: 100%;
  border: 1px solid var(--line);
  background: #061811;
  color: var(--text);
  padding: 11px 12px;
  border-radius: 10px;
}

.hidden {
  display: none !important;
}

.status {
  padding: 10px 12px;
  border-radius: 10px;
  margin: 12px 0;
  white-space: pre-wrap;
}

.status.ok {
  background: #174b32;
  color: #bff5d2;
}

.status.err {
  background: #542727;
  color: #ffd1d1;
}

.table-wrap {
  overflow: auto;
}

table {
  width: 100%;
  border-collapse: collapse;
  min-width: 520px;
}

th, td {
  text-align: left;
  padding: 11px 9px;
  border-bottom: 1px solid var(--line);
}

th {
  color: var(--gold2);
}

td {
  color: var(--muted);
}

.pill {
  display: inline-block;
  border-radius: 99px;
  padding: 3px 9px;
  background: #174b32;
  color: #bff5d2;
  font-size: .8rem;
}

.footer {
  border-top: 1px solid var(--line);
  padding: 24px 0;
  color: var(--muted);
  text-align: center;
  margin-top: 30px;
}

@media (max-width: 800px) {
  .hero,
  .admin-layout {
    grid-template-columns: 1fr;
  }

  .grid3 {
    grid-template-columns: 1fr;
  }

  .nav {
    align-items: flex-start;
    flex-direction: column;
    padding: 12px 0;
  }
}

@media (max-width: 460px) {
  .stats {
    grid-template-columns: 1fr;
  }

  .hero h1 {
    font-size: 2.15rem;
  }
}
</style>
</head>

<body>
<header class="topbar">
  <nav class="nav wrap">
    <div class="brand">
      <div class="logo">እ</div>
      <span>
        አለማየሁ እቁብ<br>
        <small class="muted">Alemayehu Equb</small>
      </span>
    </div>

    <div class="navlinks">
      <a href="#home">መነሻ</a>
      <a href="#about">ስለ እቁብ</a>
      <a href="#notices">ማስታወቂያ</a>
      <a href="#admin">Admin</a>
    </div>
  </nav>
</header>

<main>
<section id="home" class="wrap hero">
  <div>
    <div class="eyebrow">እምነት • ቁጠባ • አንድነት</div>

    <h1>
      በአንድነት እንቆጥብ፣<br>
      <span>በእምነት እንደግፍ።</span>
    </h1>

    <p class="lead">
      አለማየሁ እቁብ የአባላትን መረጃ፣
      የክፍያ ሁኔታ እና ማስታወቂያዎችን
      ለማስተዳደር የተዘጋጀ ዘመናዊ መድረክ ነው።
    </p>

    <div class="actions">
      <a class="btn btn-primary" href="#notices">ማስታወቂያዎችን ተመልከት</a>
      <a class="btn btn-ghost" href="#admin">የአስተዳዳሪ መግቢያ</a>
    </div>
  </div>

  <aside class="hero-card">
    <div class="coin">እ</div>
    <h3>አለማየሁ እቁብ</h3>
    <p class="muted">
      በግልጽነት የሚመራ፣ በአባላት እምነት
      የሚጠናከር የቁጠባ ማህበር።
    </p>
  </aside>
</section>

<section class="wrap stats">
  <div class="stat">
    <strong id="publicNoticeCount">—</strong>
    <span>ማስታወቂያዎች</span>
  </div>
  <div class="stat">
    <strong>24/7</strong>
    <span>የመረጃ መዳረሻ</span>
  </div>
  <div class="stat">
    <strong>🔐</strong>
    <span>የአስተዳዳሪ መግቢያ</span>
  </div>
</section>

<section id="about" class="wrap section">
  <h2>ስለ አለማየሁ እቁብ</h2>
  <div class="grid3">
    <article class="card">
      <div class="feature-icon">👥</div>
      <h3>የአባላት አስተዳደር</h3>
      <p class="muted">የአባላትን መረጃ በተደራጀ ሁኔታ ማስቀመጥ።</p>
    </article>

    <article class="card">
      <div class="feature-icon">💰</div>
      <h3>የክፍያ ክትትል</h3>
      <p class="muted">የሳምንት መዋጮ ክፍያዎችን መከታተል።</p>
    </article>

    <article class="card">
      <div class="feature-icon">📣</div>
      <h3>ማስታወቂያ</h3>
      <p class="muted">የእቁብ መረጃዎችን ለአባላት ማሳወቅ።</p>
    </article>
  </div>
</section>

<section id="notices" class="wrap section">
  <h2>የቅርብ ጊዜ ማስታወቂያዎች</h2>
  <div id="noticeList" class="notice-list">
    <div class="card">ማስታወቂያዎች በመጫን ላይ…</div>
  </div>
</section>

<section id="admin" class="wrap section">
  <h2>የአስተዳዳሪ መቆጣጠሪያ</h2>

  <div class="admin-layout">
    <div class="card">
      <h3>ወደ አስተዳዳሪ ግባ</h3>

      <form id="loginForm">
        <div class="field">
          <label for="email">Username</label>
          <input id="email" type="text" required placeholder="admin">
        </div>

        <div class="field">
          <label for="password">Password</label>
          <input id="password" type="password" required>
        </div>

        <button class="btn btn-primary" type="submit">ግባ</button>
      </form>

      <div id="authStatus" class="status hidden"></div>
    </div>

    <div id="adminTools" class="card hidden">
      <h3>አዲስ አባል መዝግብ</h3>

      <form id="memberForm">
        <div class="field">
          <label for="memberName">ሙሉ ስም</label>
          <input id="memberName" required>
        </div>

        <div class="field">
          <label for="memberPhone">ስልክ ቁጥር</label>
          <input id="memberPhone">
        </div>

        <div class="field">
          <label for="monthlyAmount">የሳምንት መዋጮ</label>
          <input id="monthlyAmount" type="number" value="10000" min="0" required>
        </div>

        <button class="btn btn-primary" type="submit">አባል መዝግብ</button>
      </form>

      <h3>የክፍያ መዝገብ</h3>
      <form id="paymentForm">
        <div class="field">
          <label for="paymentMember">አባል</label>
          <select id="paymentMember" required></select>
        </div>

        <div class="field">
          <label for="paymentWeek">የክፍያ ሳምንት</label>
          <input id="paymentWeek" placeholder="2026-W44" required>
        </div>

        <div class="field">
          <label for="paymentAmount">የተከፈለ መጠን</label>
          <input id="paymentAmount" type="number" min="1" required>
        </div>

        <button class="btn btn-primary" type="submit">ክፍያ መዝግብ</button>
      </form>

      <h3>የእጣ ማውጣት</h3>
      <button class="btn btn-primary" id="drawBtn" type="button">🎲 እጣ አውጣ</button>
      <div id="winnerBox" class="card"></div>

      <h3>አዲስ ማስታወቂያ</h3>
      <form id="noticeForm">
        <div class="field">
          <label for="noticeTitle">ርዕስ</label>
          <input id="noticeTitle" required>
        </div>
        <div class="field">
          <label for="noticeBody">መልዕክት</label>
          <textarea id="noticeBody" required></textarea>
        </div>
        <button class="btn btn-primary" type="submit">ማስታወቂያ አትም</button>
      </form>
    </div>
  </div>
</section>

<section id="records" class="wrap section hidden">
  <div class="card">
    <h2>የአባላት መዝገብ</h2>
    <div class="table-wrap">
      <table>
        <thead>
          <tr>
            <th>ስም</th>
            <th>ስልክ</th>
            <th>የሳምንት መዋጮ</th>
          </tr>
        </thead>
        <tbody id="memberTable"></tbody>
      </table>
    </div>
  </div>

  <div class="card">
    <h2>የክፍያ ታሪክ</h2>
    <div class="table-wrap">
      <table>
        <thead>
          <tr>
            <th>አባል</th>
            <th>ሳምንት</th>
            <th>መጠን</th>
          </tr>
        </thead>
        <tbody id="paymentTable"></tbody>
      </table>
    </div>
  </div>

  <div class="card">
    <h2>የእጣ ታሪክ</h2>
    <div class="table-wrap">
      <table>
        <thead>
          <tr>
            <th>አሸናፊ</th>
            <th>ገንዘብ</th>
            <th>ቀን</th>
          </tr>
        </thead>
        <tbody id="drawTable"></tbody>
      </table>
    </div>
  </div>
</section>
</main>

<footer class="footer">
  © <span id="year"></span>
  <strong>አለማየሁ እቁብ</strong>
</footer>

<script type="module">
import { initializeApp } from
  "https://www.gstatic.com/firebasejs/10.12.2/firebase-app.js";

import {
  getAuth,
  signInWithEmailAndPassword,
  onAuthStateChanged,
  signOut
} from "https://www.gstatic.com/firebasejs/10.12.2/firebase-auth.js";

import {
  getDatabase,
  ref,
  push,
  set,
  onValue
} from "https://www.gstatic.com/firebasejs/10.12.2/firebase-database.js";

/*
  Firebase configuration.
  Database Rules በFirebase Console ውስጥ
  በደህንነት መዋቀር አለባቸው።
*/
const firebaseConfig = {
  apiKey: "AIzaSyCrw9iYsLyW-5QNLw8dQtX0bHUFb-RZfyA",
  authDomain: "alemayehu-equb.firebaseapp.com",
  databaseURL: "https://alemayehu-equb-default-rtdb.firebaseio.com",
  projectId: "alemayehu-equb",
  storageBucket: "alemayehu-equb.firebasestorage.app",
  messagingSenderId: "901654220346",
  appId: "1:901654220346:web:f7663e1f34ebe43dcf2f03",
  measurementId: "G-GGMKD16XWD"
};

const ADMIN_UID = "4wKzPoWrRdhysvdz8ufYpNoEebj2";

const app = initializeApp(firebaseConfig);
const auth = getAuth(app);
const db = getDatabase(app);

const $ = id => document.getElementById(id);

const state = {
  members: {},
  payments: {},
  draws: {},
  user: null
};

$("year").textContent = new Date().getFullYear();

function isAdmin(user) {
  return Boolean(user && user.uid === ADMIN_UID);
}

function money(value) {
  return Number(value || 0).toLocaleString("en-US") + " ብር";
}

function showStatus(message, type = "info") {
  const el = $("authStatus");
  el.textContent = message;
  el.className = "status " + type;
}

$("loginForm").addEventListener("submit", async event => {
  event.preventDefault();

  try {
    const username = $("email").value.trim();
    const email = username.toLowerCase() === "admin"
      ? "agizachew238@gmail.com"
      : username;

    await signInWithEmailAndPassword(
      auth,
      email,
      $("password").value
    );
  } catch (error) {
    showStatus(
      "መግባት አልተሳካም። Firebase Authentication እና የመግቢያ መረጃውን ያረጋግጡ።",
      "err"
    );
    console.error(error);
  }
});

$("logoutBtn")?.addEventListener("click", async () => {
  await signOut(auth);
});

onAuthStateChanged(auth, user => {
  state.user = user;

  const admin = isAdmin(user);

  $("adminTools").classList.toggle("hidden", !admin);
  $("records").classList.toggle("hidden", !admin);
});

onValue(ref(db, "notices"), snapshot => {
  const notices = Object.values(snapshot.val() || {});

  $("publicNoticeCount").textContent = notices.length;

  $("noticeList").innerHTML = notices
    .sort((a, b) => (b.createdAt || 0) - (a.createdAt || 0))
    .map(notice => `
      <article class="notice">
        <strong>${escapeHTML(notice.title || "")}</strong>
        <p>${escapeHTML(notice.body || "")}</p>
      </article>
    `).join("") || "<div class='card'>ማስታወቂያ የለም።</div>";
});

function escapeHTML(value) {
  return String(value).replace(/[&<>"']/g, char => ({
    "&": "&amp;",
    "<": "&lt;",
    ">": "&gt;",
    '"': "&quot;",
    "'": "&#39;"
  })[char]);
}

/* አዲስ አባል መመዝገብ */
$("memberForm").addEventListener("submit", async event => {
  event.preventDefault();

  if (!isAdmin(auth.currentUser)) {
    return showStatus("የአስተዳዳሪ ፈቃድ ያስፈልጋል።", "err");
  }

  const name = $("memberName").value.trim();
  const phone = $("memberPhone").value.trim();
  const amount = Number($("monthlyAmount").value);

  if (!name || amount < 0) {
    return showStatus("የአባሉን መረጃ ያረጋግጡ።", "err");
  }

  try {
    const memberRef = push(ref(db, "members"));

    await set(memberRef, {
      name,
      phone,
      monthlyAmount: amount,
      status: "active",
      createdAt: Date.now(),
      createdBy: auth.currentUser.uid
    });

    $("memberForm").reset();

    showStatus("አባሉ ተመዝግቧል።", "ok");
  } catch (error) {
    showStatus("አባል መመዝገብ አልተቻለም።", "err");
    console.error(error);
  }
});

/* የክፍያ መዝገብ */
$("paymentForm").addEventListener("submit", async event => {
  event.preventDefault();

  if (!isAdmin(auth.currentUser)) {
    return showStatus("የአስተዳዳሪ ፈቃድ ያስፈልጋል።", "err");
  }

  const memberId = $("paymentMember").value;
  const week = $("paymentWeek").value.trim();
  const amount = Number($("paymentAmount").value);

  if (!memberId || !/^\d{4}-W\d{2}$/.test(week) || amount <= 0) {
    return showStatus("የክፍያ መረጃውን ያረጋግጡ።", "err");
  }

  try {
    const paymentRef = push(ref(db, "payments"));

    await set(paymentRef, {
      memberId,
      week,
      amount,
      createdAt: Date.now(),
      createdBy: auth.currentUser.uid
    });

    $("paymentForm").reset();

    showStatus("ክፍያው ተመዝግቧል።", "ok");
  } catch (error) {
    showStatus("ክፍያውን መመዝገብ አልተቻለም።", "err");
    console.error(error);
  }
});

/* ማስታወቂያ ማተም */
$("noticeForm").addEventListener("submit", async event => {
  event.preventDefault();

  if (!isAdmin(auth.currentUser)) {
    return showStatus("የአስተዳዳሪ ፈቃድ ያስፈልጋል።", "err");
  }

  const title = $("noticeTitle").value.trim();
  const body = $("noticeBody").value.trim();

  try {
    const noticeRef = push(ref(db, "notices"));

    await set(noticeRef, {
      title,
      body,
      createdAt: Date.now(),
      createdBy: auth.currentUser.uid
    });

    $("noticeForm").reset();

    showStatus("ማስታወቂያው ታትሟል።", "ok");
  } catch (error) {
    showStatus("ማስታወቂያውን ማተም አልተቻለም።", "err");
    console.error(error);
  }
});

/* የእጣ ማውጣት */
$("drawBtn").addEventListener("click", async () => {
  if (!isAdmin(auth.currentUser)) {
    return showStatus("የአስተዳዳሪ ፈቃድ ያስፈልጋል።", "err");
  }

  const members = Object.entries(state.members)
    .filter(([, member]) => member.status === "active");

  if (!members.length) {
    return showStatus("ንቁ አባላት አልተገኙም።", "err");
  }

  const index = Math.floor(Math.random() * members.length);
  const [memberId, winner] = members[index];

  const drawRef = push(ref(db, "draws"));

  await set(drawRef, {
    winnerId: memberId,
    winnerName: winner.name,
    potAmount: members.length * 10000,
    createdAt: Date.now(),
    createdBy: auth.currentUser.uid
  });

  $("winnerBox").textContent =
    "የእጣው አሸናፊ፦ " + winner.name +
    " | የእጣ ገንዘብ፦ " + money(members.length * 10000);
});

/* ከFirebase የአባላት መረጃ ማምጣት */
onValue(ref(db, "members"), snapshot => {
  state.members = snapshot.val() || {};

  $("memberTable").innerHTML = Object.entries(state.members)
    .map(([id, member]) => `
      <tr>
        <td>${escapeHTML(member.name || "")}</td>
        <td>${escapeHTML(member.phone || "")}</td>
        <td>${money(member.monthlyAmount)}</td>
      </tr>
    `).join("");

  $("paymentMember").innerHTML =
    '<option value="">አባል ይምረጡ</option>' +
    Object.entries(state.members).map(([id, member]) => `
      <option value="${escapeHTML(id)}">
        ${escapeHTML(member.name || "")}
      </option>
    `).join("");
});

/* የክፍያ ታሪክ */
onValue(ref(db, "payments"), snapshot => {
  state.payments = snapshot.val() || {};

  $("paymentTable").innerHTML = Object.values(state.payments)
    .map(payment => `
      <tr>
        <td>${escapeHTML(state.members[payment.memberId]?.name || "")}</td>
        <td>${escapeHTML(payment.week || "")}</td>
        <td>${money(payment.amount)}</td>
      </tr>
    `).join("");
});

/* የእጣ ታሪክ */
onValue(ref(db, "draws"), snapshot => {
  state.draws = snapshot.val() || {};

  $("drawTable").innerHTML = Object.values(state.draws)
    .map(draw => `
      <tr>
        <td>${escapeHTML(draw.winnerName || "")}</td>
        <td>${money(draw.potAmount)}</td>
        <td>${new Date(draw.createdAt).toLocaleDateString()}</td>
      </tr>
    `).join("");<script type="module">
  import { initializeApp } from "https://www.gstatic.com/firebasejs/11.10.0/firebase-app.js";

  import {
    getAuth,
    signInWithEmailAndPassword,
    signOut
  } from "https://www.gstatic.com/firebasejs/11.10.0/firebase-auth.js";

  import {
    getDatabase,
    ref,
    get,
    set,
    push,
    onValue
  } from "https://www.gstatic.com/firebasejs/11.10.0/firebase-database.js";

  const firebaseConfig = {
    apiKey: "AIzaSyCrw9iYsLyW-5QNLw8dQtX0bHUFb-RZfyA",
    authDomain: "alemayehu-equb.firebaseapp.com",
    databaseURL: "https://alemayehu-equb-c3d70-default-rtdb.firebaseio.com",
    projectId: "alemayehu-equb",
    storageBucket: "alemayehu-equb.firebasestorage.app",
    messagingSenderId: "901654220346",
    appId: "1:901654220346:web:f1185006a2279069cf2f03"
  };

  const app = initializeApp(firebaseConfig);
  const auth = getAuth(app);
  const db = getDatabase(app);

  window.equbFirebase = {
    app,
    auth,
    db,
    signInWithEmailAndPassword,
    signOut,
    ref,
    get,
    set,
    push,
    onValue
  };

  console.log("Alemayehu Equb Firebase initialized.");
</script>
});
</script>
</body>
</html>
