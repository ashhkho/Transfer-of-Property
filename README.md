[tpa_chapters_1_4.html](https://github.com/user-attachments/files/28918605/tpa_chapters_1_4.html)
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Transfer of Property Act 1882 — Chapters I–IV</title>
<style>
  @import url('https://fonts.googleapis.com/css2?family=EB+Garamond:ital,wght@0,400;0,500;0,600;1,400&family=DM+Mono:wght@400;500&display=swap');

  :root {
    --bg: #faf8f4;
    --surface: #ffffff;
    --surface2: #f4f1eb;
    --border: #e0d9ce;
    --border2: #ccc4b8;
    --ink: #1a1714;
    --ink2: #4a4540;
    --ink3: #7a746e;
    --accent: #7c3a1e;
    --accent2: #a84c28;
    --accent-bg: #fdf0ea;
    --ch1: #2d5a8e;
    --ch1bg: #eef4fb;
    --ch2: #1e6b4a;
    --ch2bg: #eaf5f0;
    --ch3: #7c4a1e;
    --ch3bg: #fdf1e8;
    --ch4: #5a2d8e;
    --ch4bg: #f3eefb;
    --tag-cannot: #8e2d2d;
    --tag-cannot-bg: #fbeaea;
    --tag-void: #8e6b1e;
    --tag-void-bg: #fbf5ea;
    --tag-key: #1e4d8e;
    --tag-key-bg: #eaf0fb;
    --tag-doctrine: #2d7a3a;
    --tag-doctrine-bg: #eaf5ec;
  }

  * { box-sizing: border-box; margin: 0; padding: 0; }

  body {
    font-family: 'EB Garamond', Georgia, serif;
    background: var(--bg);
    color: var(--ink);
    font-size: 15px;
    line-height: 1.65;
  }

  /* HEADER */
  header {
    background: var(--ink);
    color: #faf8f4;
    padding: 32px 48px 28px;
    border-bottom: 3px solid var(--accent);
  }
  header h1 {
    font-size: 28px;
    font-weight: 600;
    letter-spacing: 0.02em;
    margin-bottom: 6px;
  }
  header p {
    font-size: 14px;
    color: #b8b0a4;
    font-style: italic;
  }
  header .meta {
    display: flex; gap: 20px; margin-top: 16px; flex-wrap: wrap;
  }
  header .meta span {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    background: rgba(255,255,255,0.08);
    padding: 4px 10px;
    border-radius: 3px;
    letter-spacing: 0.05em;
    color: #d4cdc6;
  }

  /* CONTROLS */
  .controls {
    position: sticky; top: 0; z-index: 100;
    background: var(--surface);
    border-bottom: 1px solid var(--border);
    padding: 12px 48px;
    display: flex; align-items: center; gap: 16px; flex-wrap: wrap;
  }
  .controls label { font-size: 12px; font-family: 'DM Mono', monospace; color: var(--ink3); text-transform: uppercase; letter-spacing: 0.06em; }
  .search-box {
    padding: 6px 14px;
    border: 1px solid var(--border2);
    border-radius: 4px;
    font-family: 'EB Garamond', serif;
    font-size: 14px;
    background: var(--bg);
    color: var(--ink);
    width: 220px;
    outline: none;
  }
  .search-box:focus { border-color: var(--accent); }
  .filter-btns { display: flex; gap: 6px; flex-wrap: wrap; }
  .filter-btn {
    padding: 4px 12px;
    border: 1px solid var(--border2);
    border-radius: 20px;
    background: var(--bg);
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    cursor: pointer;
    color: var(--ink2);
    letter-spacing: 0.04em;
    transition: all 0.15s;
  }
  .filter-btn:hover { border-color: var(--accent); color: var(--accent); }
  .filter-btn.active { background: var(--ink); color: #fff; border-color: var(--ink); }
  .count-label { font-family: 'DM Mono', monospace; font-size: 11px; color: var(--ink3); margin-left: auto; }

  /* CHAPTER GROUPS */
  .chapter-group { margin: 0; }
  .chapter-header {
    display: flex; align-items: center; gap: 14px;
    padding: 14px 48px;
    border-top: 2px solid;
    cursor: pointer;
    user-select: none;
    background: var(--surface2);
    position: sticky; top: 57px; z-index: 90;
  }
  .chapter-header:hover { filter: brightness(0.97); }
  .ch-roman { font-family: 'DM Mono', monospace; font-size: 13px; font-weight: 500; letter-spacing: 0.08em; }
  .ch-title { font-size: 17px; font-weight: 600; }
  .ch-range { font-family: 'DM Mono', monospace; font-size: 11px; margin-left: auto; color: inherit; opacity: 0.65; }
  .ch-toggle { font-size: 12px; opacity: 0.5; }

  .ch1 .chapter-header { border-color: var(--ch1); color: var(--ch1); }
  .ch2 .chapter-header { border-color: var(--ch2); color: var(--ch2); }
  .ch3 .chapter-header { border-color: var(--ch3); color: var(--ch3); }
  .ch4 .chapter-header { border-color: var(--ch4); color: var(--ch4); }

  /* TABLE */
  .table-wrap { overflow-x: auto; }
  table {
    width: 100%;
    border-collapse: collapse;
    font-size: 14px;
  }
  thead tr {
    background: var(--ink);
    color: #faf8f4;
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    letter-spacing: 0.06em;
    text-transform: uppercase;
  }
  thead th {
    padding: 10px 16px;
    text-align: left;
    font-weight: 500;
    white-space: nowrap;
  }
  tbody tr {
    border-bottom: 1px solid var(--border);
    transition: background 0.1s;
  }
  tbody tr:hover { background: var(--accent-bg); }
  tbody tr.hidden { display: none; }
  td {
    padding: 13px 16px;
    vertical-align: top;
  }

  /* Column widths */
  .col-sec   { width: 90px; white-space: nowrap; }
  .col-name  { width: 170px; }
  .col-concept { width: 130px; }
  .col-ingr  { width: 200px; }
  .col-expl  { width: 230px; }
  .col-illus { width: 210px; }
  .col-read  { width: 110px; }

  /* Section badge */
  .sec-badge {
    display: inline-block;
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    font-weight: 500;
    padding: 3px 8px;
    border-radius: 3px;
    letter-spacing: 0.04em;
    white-space: nowrap;
  }
  .ch1 .sec-badge { background: var(--ch1bg); color: var(--ch1); }
  .ch2 .sec-badge { background: var(--ch2bg); color: var(--ch2); }
  .ch3 .sec-badge { background: var(--ch3bg); color: var(--ch3); }
  .ch4 .sec-badge { background: var(--ch4bg); color: var(--ch4); }

  /* Section name */
  .sec-name { font-weight: 600; font-size: 13.5px; line-height: 1.4; }

  /* Tags */
  .tag {
    display: inline-block;
    font-family: 'DM Mono', monospace;
    font-size: 10px;
    padding: 1px 6px;
    border-radius: 2px;
    margin-top: 4px;
    letter-spacing: 0.04em;
  }
  .tag-cannot { background: var(--tag-cannot-bg); color: var(--tag-cannot); }
  .tag-void   { background: var(--tag-void-bg); color: var(--tag-void); }
  .tag-key    { background: var(--tag-key-bg); color: var(--tag-key); }
  .tag-doctrine { background: var(--tag-doctrine-bg); color: var(--tag-doctrine); }

  /* Ingredient list */
  .ingr-list { padding-left: 0; list-style: none; }
  .ingr-list li { padding: 1px 0 1px 12px; position: relative; font-size: 13.5px; line-height: 1.5; }
  .ingr-list li::before { content: '—'; position: absolute; left: 0; color: var(--ink3); font-size: 11px; top: 3px; }

  /* Explanation */
  .expl { font-size: 13.5px; color: var(--ink2); line-height: 1.55; }
  .expl strong { color: var(--ink); font-weight: 600; }

  /* Illustration */
  .illus {
    font-size: 12.5px;
    font-style: italic;
    color: var(--ink2);
    background: var(--surface2);
    border-left: 2px solid var(--border2);
    padding: 7px 10px;
    border-radius: 0 4px 4px 0;
    line-height: 1.5;
  }
  .illus strong { font-style: normal; font-size: 11px; font-family: 'DM Mono', monospace; text-transform: uppercase; letter-spacing: 0.04em; color: var(--ink3); display: block; margin-bottom: 3px; }

  /* Read with */
  .read-with { font-family: 'DM Mono', monospace; font-size: 11px; line-height: 1.8; color: var(--ink3); }
  .read-with a { color: var(--accent2); text-decoration: none; border-bottom: 1px dotted var(--accent2); cursor: pointer; }
  .read-with a:hover { color: var(--accent); }

  /* Repeal notice */
  .repealed {
    font-family: 'DM Mono', monospace;
    font-size: 11px;
    color: var(--ink3);
    font-style: italic;
  }

  /* No results */
  .no-results {
    text-align: center;
    padding: 60px 20px;
    color: var(--ink3);
    font-style: italic;
    font-size: 16px;
    display: none;
  }

  /* Footer */
  footer {
    padding: 24px 48px;
    border-top: 1px solid var(--border);
    font-size: 12px;
    color: var(--ink3);
    font-style: italic;
    text-align: center;
  }
</style>
</head>
<body>

<header>
  <h1>Transfer of Property Act, 1882</h1>
  <p>Section-wise Reference Table · Chapters I through IV</p>
  <div class="meta">
    <span>ACT NO. 4 OF 1882</span>
    <span>IN FORCE: 1 JULY 1882</span>
    <span>CH. I–IV · SS. 1–104</span>
    <span>ALL SECTIONS COVERED</span>
  </div>
</header>

<div class="controls">
  <label>Search</label>
  <input class="search-box" type="text" id="searchInput" placeholder="section, concept, keyword…" oninput="filterTable()">
  <div class="filter-btns">
    <button class="filter-btn active" onclick="setFilter('all', this)">All</button>
    <button class="filter-btn" onclick="setFilter('ch1', this)">Ch. I</button>
    <button class="filter-btn" onclick="setFilter('ch2', this)">Ch. II</button>
    <button class="filter-btn" onclick="setFilter('ch3', this)">Ch. III</button>
    <button class="filter-btn" onclick="setFilter('ch4', this)">Ch. IV</button>
    <button class="filter-btn" onclick="setFilter('key', this)">⭐ Key</button>
    <button class="filter-btn" onclick="setFilter('void', this)">Void rules</button>
    <button class="filter-btn" onclick="setFilter('doctrine', this)">Doctrines</button>
  </div>
  <span class="count-label" id="countLabel"></span>
</div>

<!-- ═══════════════════════════════════════════════════════ CHAPTER I -->
<div class="chapter-group ch1" id="grp-ch1">
  <div class="chapter-header" onclick="toggleChapter('ch1')">
    <span class="ch-roman">CHAPTER I</span>
    <span class="ch-title">Preliminary</span>
    <span class="ch-range">Sections 1–4</span>
    <span class="ch-toggle" id="tog-ch1">▼</span>
  </div>
  <div class="table-wrap" id="body-ch1">
    <table>
      <thead>
        <tr>
          <th class="col-sec">Section</th>
          <th class="col-name">Section Name (Bare Act)</th>
          <th class="col-concept">Concept</th>
          <th class="col-ingr">Ingredients / Requirements</th>
          <th class="col-expl">Simple Explanation</th>
          <th class="col-illus">Illustration</th>
          <th class="col-read">Read With</th>
        </tr>
      </thead>
      <tbody>

        <tr data-ch="ch1" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 1</span></td>
          <td class="col-name"><div class="sec-name">Short title, Commencement, Extent</div></td>
          <td class="col-concept">Jurisdiction &amp; applicability</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Short title: Transfer of Property Act, 1882</li>
              <li>Came into force: 1 July 1882</li>
              <li>Extends to whole of India (with some excluded territories historically)</li>
              <li>Ss. 54(para 2,3), 59, 107, 123 cannot extend to areas excluded from Registration Act</li>
            </ul>
          </td>
          <td class="col-expl expl">Tells you the name of the Act, when it started, and where it applies. Some sections require registration infrastructure to work — so they can only apply where the Registration Act applies.</td>
          <td class="col-illus"><div class="illus"><strong>Note</strong>Madhya Pradesh is within the Act's territory. The Act came into force before the Constitution — many territorial amendments were made post-independence.</div></td>
          <td class="col-read"><div class="read-with">Indian Registration Act, 1908</div></td>
        </tr>

        <tr data-ch="ch1" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 2</span></td>
          <td class="col-name"><div class="sec-name">Repeal of Acts. Saving of certain enactments, incidents, rights, liabilities, etc.</div></td>
          <td class="col-concept">Savings clause</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Repeals earlier enactments listed in the Schedule</li>
              <li>But does NOT affect: other unrepealed enactments; contractual terms consistent with this Act; rights/liabilities from before this Act; transfers by operation of law or court decree; rules of Muhammadan law (Ch. II)</li>
            </ul>
          </td>
          <td class="col-expl expl">Earlier property laws are repealed, but existing rights and legal relations formed before 1882 are protected. Muslim personal law regarding property is also unaffected by Chapter II.</td>
          <td class="col-illus"><div class="illus"><strong>Note</strong>If A held a right in property arising from a contract made in 1875 (before the Act), that right is preserved even after the Act came into force.</div></td>
          <td class="col-read"><div class="read-with">The Schedule (list of repealed Acts)</div></td>
        </tr>

        <tr data-ch="ch1" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 3</span></td>
          <td class="col-name"><div class="sec-name">Interpretation-clause</div><div><span class="tag tag-key">KEY DEFINITIONS</span></div></td>
          <td class="col-concept">Definitions</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li><strong>Immoveable property:</strong> excludes standing timber, growing crops, grass</li>
              <li><strong>Instrument:</strong> non-testamentary instrument only</li>
              <li><strong>Attested:</strong> signed by 2+ witnesses, each having seen executant sign or received personal acknowledgment; each signed in executant's presence</li>
              <li><strong>Registered:</strong> registered under Indian Registration Act in the territories</li>
              <li><strong>Attached to the earth:</strong> (a) rooted — trees, shrubs; (b) embedded — walls, buildings; (c) attached to embedded thing for permanent beneficial enjoyment</li>
              <li><strong>Actionable claim:</strong> claim to unsecured debt, or beneficial interest in moveable property not in claimant's possession, recognised by civil courts</li>
              <li><strong>Notice:</strong> actual knowledge, OR wilful abstention from inquiry / gross negligence (constructive notice). Expl. I: registered instrument = notice from date of registration. Expl. II: actual possessor's title = notice. Expl. III: agent's notice = principal's notice (unless agent fraudulently conceals)</li>
            </ul>
          </td>
          <td class="col-expl expl">These definitions govern how words are understood throughout the Act. <strong>Notice</strong> is particularly important — you are deemed to know what you would have known with reasonable diligence. Willful ignorance = constructive notice.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (Notice)</strong>B is about to buy land from A. The land is registered in A's name but C is actually living on it. B is deemed to have notice of C's title (Expl. II), even if B never asked C about it.</div></td>
          <td class="col-read"><div class="read-with">S. 55(1)(a) — seller's duty to disclose<br>S. 41 — ostensible owner<br>Indian Registration Act, 1908 (S. 51, 55)</div></td>
        </tr>

        <tr data-ch="ch1" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 4</span></td>
          <td class="col-name"><div class="sec-name">Enactments relating to contracts to be taken as part of Contract Act and supplemental to the Registration Act</div></td>
          <td class="col-concept">Relationship with other Acts</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Chapters/sections relating to contracts = part of Indian Contract Act, 1872</li>
              <li>Ss. 54 (para 2, 3), 59, 107, 123 = supplemental to Indian Registration Act, 1908</li>
            </ul>
          </td>
          <td class="col-expl expl">This Act does not stand alone — its contract-related provisions are treated as part of the Contract Act, and key sections on sale, mortgage, lease, and gift are read alongside the Registration Act. All three Acts must be read together for property transactions.</td>
          <td class="col-illus"><div class="illus"><strong>Note</strong>A contract for sale of land (S. 54 para 3) uses Contract Act principles (offer, acceptance, consideration) but is supplemented by Registration Act requirements.</div></td>
          <td class="col-read"><div class="read-with">Indian Contract Act, 1872<br>Indian Registration Act, 1908</div></td>
        </tr>

      </tbody>
    </table>
  </div>
</div>

<!-- ═══════════════════════════════════════════════════════ CHAPTER II -->
<div class="chapter-group ch2" id="grp-ch2">
  <div class="chapter-header" onclick="toggleChapter('ch2')">
    <span class="ch-roman">CHAPTER II</span>
    <span class="ch-title">Of Transfers of Property by Act of Parties</span>
    <span class="ch-range">Sections 5–53A</span>
    <span class="ch-toggle" id="tog-ch2">▼</span>
  </div>
  <div class="table-wrap" id="body-ch2">
    <table>
      <thead>
        <tr>
          <th class="col-sec">Section</th>
          <th class="col-name">Section Name (Bare Act)</th>
          <th class="col-concept">Concept</th>
          <th class="col-ingr">Ingredients / Requirements</th>
          <th class="col-expl">Simple Explanation</th>
          <th class="col-illus">Illustration</th>
          <th class="col-read">Read With</th>
        </tr>
      </thead>
      <tbody>

        <tr data-ch="ch2" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 5</span></td>
          <td class="col-name"><div class="sec-name">"Transfer of property" defined</div><div><span class="tag tag-key">DEFINITION</span></div></td>
          <td class="col-concept">Transfer defined</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Act by a <strong>living person</strong></li>
              <li>Conveys property — present or future</li>
              <li>To one or more other living persons, or to himself, or to himself and others</li>
              <li>"Living person" includes companies, associations, bodies of individuals (incorporated or not)</li>
            </ul>
          </td>
          <td class="col-expl expl">Only a living person can transfer property — this excludes transfers by will (done on death). The transfer can be immediate or in future. A company counts as a "living person."</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A (a company) sells its factory to B. Valid — company is a "living person." But if A writes in his will that his farm goes to B, that is NOT a transfer under this Act — it takes effect on death and is governed by succession law.</div></td>
          <td class="col-read"><div class="read-with">S. 6 — what may be transferred<br>S. 7 — who can transfer</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key cannot">
          <td class="col-sec"><span class="sec-badge">S. 6</span></td>
          <td class="col-name"><div class="sec-name">What may be transferred</div><div><span class="tag tag-cannot">NON-TRANSFERABLE</span></div></td>
          <td class="col-concept">Transferable &amp; non-transferable property</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li><strong>General rule:</strong> any property may be transferred</li>
              <li><strong>(a)</strong> Spes successionis (heir's chance, legacy chance) — cannot transfer</li>
              <li><strong>(b)</strong> Mere right of re-entry for breach of condition subsequent — cannot transfer (except to property owner)</li>
              <li><strong>(c)</strong> Easement — cannot transfer apart from dominant heritage</li>
              <li><strong>(d)</strong> Interest restricted to personal enjoyment — cannot transfer</li>
              <li><strong>(dd)</strong> Right to future maintenance — cannot transfer</li>
              <li><strong>(e)</strong> Mere right to sue — cannot transfer</li>
              <li><strong>(f)</strong> Public office; salary of public officer — cannot transfer</li>
              <li><strong>(g)</strong> Military, naval, air force, civil pensions; political pensions — cannot transfer</li>
              <li><strong>(h)</strong> Transfer opposed to nature of interest; unlawful object/consideration; transfer to legally disqualified person — void</li>
              <li><strong>(i)</strong> Untransferable occupancy tenant; farmer of defaulting estate; lessee under Court of Wards — cannot assign</li>
            </ul>
          </td>
          <td class="col-expl expl">Property is presumed transferable unless the Act or another law specifically prohibits it. The exceptions protect public policy (pensions, offices) and prevent speculation on uncertain future rights (spes successionis).</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (a)</strong>A's father B is alive. A "sells" his expected inheritance to C. This is void — A only has a spes successionis (mere chance), not a present right. B might change his will or spend the property.<br><br><strong>Illustration (e)</strong>A has a right to sue B for a debt. A cannot sell this right to sue to C.</div></td>
          <td class="col-read"><div class="read-with">S. 5 — transfer defined<br>S. 7 — competency<br>Indian Contract Act S. 23 (unlawful object)</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 7</span></td>
          <td class="col-name"><div class="sec-name">Persons competent to transfer</div></td>
          <td class="col-concept">Competency to transfer</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Competent to contract (major, sound mind, not disqualified)</li>
              <li>Entitled to transferable property, OR authorised to dispose of transferable property not his own</li>
              <li>Can transfer wholly or partly, absolutely or conditionally</li>
            </ul>
          </td>
          <td class="col-expl expl">You must be legally competent (as per Contract Act) to transfer. A minor cannot transfer. A guardian or agent authorised by law can transfer property that is not their own.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A (minor) tries to sell land. The transfer is void — A is not competent to contract. But A's guardian, if authorised by court, can transfer A's property.</div></td>
          <td class="col-read"><div class="read-with">Indian Contract Act, S. 11 (competency)<br>S. 6(h) — legally disqualified transferee</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 8</span></td>
          <td class="col-name"><div class="sec-name">Operation of transfer</div></td>
          <td class="col-concept">What passes on transfer</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Unless contrary intention expressed/implied, transfer passes ALL interest the transferor can pass</li>
              <li>Land: easements annexed, rents &amp; profits after transfer, things attached to earth</li>
              <li>House: easements, rent, locks, keys, bars, doors, windows, permanent fixtures</li>
              <li>Machinery (attached): moveable parts</li>
              <li>Debt/actionable claim: securities (except for other debts), NOT arrears of interest before transfer</li>
              <li>Money/income-yielding property: income accruing after transfer</li>
            </ul>
          </td>
          <td class="col-expl expl">When you transfer property, everything that goes along with it (its legal accessories) also transfers automatically — unless you say otherwise. A house transfer includes its keys and windows; a land transfer includes its easements.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A sells a house to B. A does not mention the main door or the easement of way over the neighbour's land. Both pass to B automatically under S. 8.</div></td>
          <td class="col-read"><div class="read-with">S. 5 — transfer defined<br>S. 55 — rights/liabilities on sale</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 9</span></td>
          <td class="col-name"><div class="sec-name">Oral transfer</div></td>
          <td class="col-concept">Mode of transfer — oral</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Transfer without writing is valid</li>
              <li>Unless writing is expressly required by law</li>
            </ul>
          </td>
          <td class="col-expl expl">Property can be transferred orally unless a specific law requires writing. For example, sale of immoveable property ≥ Rs.100 requires a registered instrument (S. 54), so oral sale is invalid there. But moveable property can be gifted by delivery (S. 123).</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A hands B a book and says "this is yours." Valid oral/delivery transfer of moveable property. But A cannot orally transfer his house to B — S. 54 requires registration.</div></td>
          <td class="col-read"><div class="read-with">S. 54 — sale (writing required)<br>S. 107 — lease (writing required &gt;1yr)<br>S. 123 — gift</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="void key">
          <td class="col-sec"><span class="sec-badge">S. 10</span></td>
          <td class="col-name"><div class="sec-name">Condition restraining alienation</div><div><span class="tag tag-void">VOID CONDITION</span></div></td>
          <td class="col-concept">Absolute restraint on alienation is void</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Condition/limitation absolutely restraining the transferee from parting with or disposing of their interest = <strong>void</strong></li>
              <li><strong>Exception 1:</strong> Lease — condition for benefit of lessor is valid</li>
              <li><strong>Exception 2:</strong> Transfer to woman (not Hindu/Muslim/Buddhist) — may be restrained from transferring during marriage</li>
            </ul>
          </td>
          <td class="col-expl expl">Once you give someone property, you cannot attach a condition saying they can NEVER sell or transfer it. That destroys the very nature of ownership. <em>Partial</em> restraints (e.g. "do not sell for 5 years") are generally valid; <em>absolute</em> restraints are void.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers land to B "on condition that B shall never sell or mortgage the land." The condition is void. B gets the land free of that restriction and can sell it.</div></td>
          <td class="col-read"><div class="read-with">S. 11 — restriction on enjoyment<br>S. 12 — insolvency condition<br>S. 105 — lease</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="void">
          <td class="col-sec"><span class="sec-badge">S. 11</span></td>
          <td class="col-name"><div class="sec-name">Restriction repugnant to interest created</div><div><span class="tag tag-void">VOID CONDITION</span></div></td>
          <td class="col-concept">Restriction on enjoyment void if absolute interest given</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Absolute interest created in favour of a person</li>
              <li>Terms direct that it be enjoyed in a <em>particular manner</em></li>
              <li>Such direction = <strong>void</strong>; person takes interest free of direction</li>
              <li><strong>Exception:</strong> direction securing beneficial enjoyment of <em>another piece of immoveable property</em> — transferor may enforce it (restrictive covenant)</li>
            </ul>
          </td>
          <td class="col-expl expl">If you give someone full (absolute) ownership, you cannot simultaneously dictate how they use or enjoy it. The two are repugnant — absolute ownership and directions for use cannot coexist. But a restrictive covenant protecting neighbouring land is enforceable.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers Rs. 10,000 to B absolutely "but B must use it only for farming." The direction is void — B can use the money however he wishes. But if A transfers Plot X to B with a condition not to build higher than 2 floors (to protect A's light on Plot Y), that is enforceable.</div></td>
          <td class="col-read"><div class="read-with">S. 10 — restraint on alienation<br>S. 40 — burden of obligation on land</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="void">
          <td class="col-sec"><span class="sec-badge">S. 12</span></td>
          <td class="col-name"><div class="sec-name">Condition making interest determinable on insolvency or attempted alienation</div><div><span class="tag tag-void">VOID CONDITION</span></div></td>
          <td class="col-concept">Forfeiture on insolvency/alienation attempt is void</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Property transferred subject to a condition</li>
              <li>Condition: interest ceases if transferee becomes insolvent OR tries to transfer/dispose of it</li>
              <li>Such condition = <strong>void</strong></li>
              <li><strong>Exception:</strong> Lease — condition for benefit of lessor is valid</li>
            </ul>
          </td>
          <td class="col-expl expl">A transferor cannot create a trap where the transferee loses the property upon becoming bankrupt or trying to sell it. This would make the "transfer" meaningless — the transferee would never truly own it. The condition is void; the interest stands.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers a house to B "on condition that if B ever goes bankrupt or tries to sell the house, it returns to A." The condition is void — B holds the house free of this condition.</div></td>
          <td class="col-read"><div class="read-with">S. 10 — restraint on alienation<br>S. 111(g) — forfeiture in leases (valid exception)</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 13</span></td>
          <td class="col-name"><div class="sec-name">Transfer for benefit of unborn person</div></td>
          <td class="col-concept">Transfer to unborn person</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest created for an unborn person</li>
              <li>Subject to a prior interest created by the same transfer</li>
              <li>Interest for unborn person is valid ONLY if it extends to the <strong>whole remaining interest</strong> of the transferor</li>
            </ul>
          </td>
          <td class="col-expl expl">You cannot give a piece of the property to an unborn person — they must get everything remaining. This prevents fragmentation of interests in favour of persons not yet born. The unborn person acquires a vested interest upon birth (S. 20).</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A transfers property to B for life, then to A's intended wife for life, then to their eldest son for life, then to second son. The interest for the eldest son fails — because it does not extend to the whole remaining interest (second son's interest was carved out).</div></td>
          <td class="col-read"><div class="read-with">S. 14 — rule against perpetuity<br>S. 20 — unborn person acquires vested interest<br>S. 16 — failure of prior interest</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 14</span></td>
          <td class="col-name"><div class="sec-name">Rule against perpetuity</div><div><span class="tag tag-key">KEY RULE</span></div></td>
          <td class="col-concept">Property cannot be tied up forever</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>No transfer can create an interest taking effect after:</li>
              <li>Lifetime of one or more persons living at date of transfer, <strong>PLUS</strong></li>
              <li>Minority of some person in existence at expiry of that period (to whom, on attaining majority, the interest belongs)</li>
              <li>Any interest created beyond this limit is <strong>void</strong></li>
            </ul>
          </td>
          <td class="col-expl expl">You cannot lock property away indefinitely for future generations. The maximum "delay" before property must vest is: lives in being + 18 years (minority). After this period, the interest must vest or it is void. This prevents property from being tied up for eternity.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers to B for life, then to B's children for life, then to B's grandchildren for life, then to B's great-grandchildren absolutely. The interest for great-grandchildren may be void as it may take effect beyond the perpetuity period (lives in being + minority).</div></td>
          <td class="col-read"><div class="read-with">S. 13 — unborn person<br>S. 15 — class gifts<br>S. 16 — failure of prior interest<br>S. 18 — public benefit exception</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 15</span></td>
          <td class="col-name"><div class="sec-name">Transfer to class some of whom come under sections 13 and 14</div></td>
          <td class="col-concept">Partial failure in class gifts</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest created for a class of persons</li>
              <li>Some members fall under S.13 or S.14 (unborn/perpetuity rules)</li>
              <li>Interest fails only for <em>those persons</em>, not the entire class</li>
            </ul>
          </td>
          <td class="col-expl expl">A class gift does not fail entirely because one or two members of the class are unborn or fall foul of the perpetuity rule. The gift survives for the valid members; only the invalid portions are cut out.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers property to "all my grandchildren living at my death." Some grandchildren are born, some may be born after A's death. The interest fails only for grandchildren not yet born who would take beyond the perpetuity limit.</div></td>
          <td class="col-read"><div class="read-with">S. 13, S. 14 — the governing rules<br>S. 16 — failure of prior interest</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 16</span></td>
          <td class="col-name"><div class="sec-name">Transfer to take effect on failure of prior interest</div></td>
          <td class="col-concept">Subsequent interest also fails</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Prior interest fails under S.13 or S.14</li>
              <li>Interest intended to take effect after/upon failure of that prior interest = also fails</li>
            </ul>
          </td>
          <td class="col-expl expl">If the main gift fails due to the unborn/perpetuity rules, the fallback gift also fails. You cannot cure an invalid prior interest by having a subsequent interest depend on it.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A creates an interest for an unborn person (void under S.13). A also creates an interest "in case that unborn person's interest fails, to C." C's interest also fails — it was conditional on the prior (void) interest.</div></td>
          <td class="col-read"><div class="read-with">S. 13, S. 14 — prior rules<br>S. 27 — conditional transfer to another on failure</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 17</span></td>
          <td class="col-name"><div class="sec-name">Direction for accumulation</div></td>
          <td class="col-concept">Limit on income accumulation</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Direction to accumulate income from transferred property</li>
              <li>Valid only for: (a) life of transferor, OR (b) 18 years from transfer — whichever is <em>longer</em></li>
              <li>Beyond that period: direction is void to the extent of excess</li>
              <li><strong>Exceptions (valid accumulation):</strong> payment of transferor's debts; provision for children/issue; preservation/maintenance of property</li>
            </ul>
          </td>
          <td class="col-expl expl">You can direct that the income from property be saved (not spent) for a limited period. But you cannot instruct the income to pile up indefinitely. After the allowed period, the property and income must be dealt with as if the accumulation period had ended.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers a farm to trustees directing income to accumulate for 30 years. The direction is void for the period beyond 18 years (or A's lifetime if longer). After 18 years (or A's death), the income must be released to the beneficiaries.</div></td>
          <td class="col-read"><div class="read-with">S. 14 — rule against perpetuity<br>S. 18 — public benefit exception</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 18</span></td>
          <td class="col-name"><div class="sec-name">Transfer in perpetuity for benefit of public</div></td>
          <td class="col-concept">Public benefit exception</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Ss. 14, 16, 17 do NOT apply to:</li>
              <li>Transfer of property for the benefit of the public in advancement of: religion, knowledge, commerce, health, safety, or any object beneficial to mankind</li>
            </ul>
          </td>
          <td class="col-expl expl">Charitable and public trusts are exempt from the perpetuity rules. A temple, hospital, university, or public welfare fund can hold property indefinitely — the rule against perpetuity does not tie up such socially beneficial arrangements.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A creates a trust to maintain a hospital in his village forever, with income accumulating until a new ward is built every 10 years. This is not void under S.14 or S.17 — it is for public health benefit.</div></td>
          <td class="col-read"><div class="read-with">S. 14, S. 16, S. 17 — rules being excepted</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 19</span></td>
          <td class="col-name"><div class="sec-name">Vested interest</div></td>
          <td class="col-concept">Vested vs. contingent interest</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest created without specifying time, OR to take effect forthwith, OR on a certain event (one that <em>must</em> happen) = <strong>vested interest</strong></li>
              <li>Vested interest NOT defeated by death of transferee before possession</li>
              <li>Postponement of enjoyment alone does NOT make it contingent</li>
              <li>Contrary intention can override — must appear from terms of transfer</li>
            </ul>
          </td>
          <td class="col-expl expl">A vested interest is an interest that has already been granted — the right exists now, even if enjoyment is delayed. Like money held in trust for a child until they turn 18 — the child has the right already; they just can't access it yet.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers property to B for life, remainder to C. C has a vested interest immediately — even though C cannot enjoy it until B dies. If C dies before B, C's interest passes to C's heirs.</div></td>
          <td class="col-read"><div class="read-with">S. 20 — unborn person gets vested interest<br>S. 21 — contingent interest<br>S. 22 — age condition</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 20</span></td>
          <td class="col-name"><div class="sec-name">When unborn person acquires vested interest on transfer for his benefit</div></td>
          <td class="col-concept">Vesting on birth</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest created for a person not then living</li>
              <li>On birth: acquires vested interest (unless contrary intention)</li>
              <li>Even if not entitled to immediate enjoyment at birth</li>
            </ul>
          </td>
          <td class="col-expl expl">The moment the unborn beneficiary is born alive, the interest vests in them — even though they may have to wait years before actually enjoying the property. Birth is the trigger for vesting.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers property to B for life, then to B's first-born child. When B's first child is born, that child gets a vested interest immediately at birth — even though they cannot enjoy it until B dies.</div></td>
          <td class="col-read"><div class="read-with">S. 13 — transfer for unborn person<br>S. 19 — vested interest</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 21</span></td>
          <td class="col-name"><div class="sec-name">Contingent interest</div></td>
          <td class="col-concept">Interest dependent on uncertain event</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest to take effect only on happening of a <em>specified uncertain event</em>, OR if it does <em>not</em> happen</li>
              <li>Becomes vested: when the event happens (former case); when event becomes impossible (latter case)</li>
              <li><strong>Exception:</strong> if transferee is entitled to income before reaching the specified age, the interest is NOT contingent</li>
            </ul>
          </td>
          <td class="col-expl expl">A contingent interest is uncertain — it may or may not ever come to exist. Like "property to B if B passes the bar exam." If B fails, the interest never arises. Compare with vested: "property to B after 5 years" — B will definitely get it, just has to wait.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers property to B "if B returns from England." B has a contingent interest — uncertain if B will return. If B returns, it vests. If B dies without returning, the interest lapses.</div></td>
          <td class="col-read"><div class="read-with">S. 19 — vested interest (compare)<br>S. 22 — age condition<br>S. 23 — contingent on uncertain event</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 22</span></td>
          <td class="col-name"><div class="sec-name">Transfer to members of a class who attain a particular age</div></td>
          <td class="col-concept">Age condition in class gift</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest for class members who attain a particular age</li>
              <li>Does NOT vest in any member who has not reached that age</li>
            </ul>
          </td>
          <td class="col-expl expl">If the gift says "to my grandchildren who reach 21," no grandchild gets a vested interest until they actually turn 21. Until then, their interest is contingent on reaching that age.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers property "to such of my children as attain the age of 25." A has three children aged 10, 20, 24. No one has a vested interest yet. When the 24-year-old turns 25, their share vests.</div></td>
          <td class="col-read"><div class="read-with">S. 19, S. 21 — vested/contingent interest</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 23</span></td>
          <td class="col-name"><div class="sec-name">Transfer contingent on happening of specified uncertain event</div></td>
          <td class="col-concept">Time limit on contingency</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest to accrue to X if uncertain event happens</li>
              <li>No time specified for occurrence</li>
              <li>Interest fails unless event happens <em>before or at same time as</em> prior/intermediate interest ceases</li>
            </ul>
          </td>
          <td class="col-expl expl">A contingent gift (dependent on an event) must materialise before the preceding interest ends. You cannot have the property sitting ownerless while waiting forever for the uncertain event.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>Property to B for life, then to C if C marries. No time for marriage is stated. C must marry before (or at the time) B dies. If B dies and C is still unmarried, C's interest fails.</div></td>
          <td class="col-read"><div class="read-with">S. 21 — contingent interest<br>S. 24 — surviving at unspecified period</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 24</span></td>
          <td class="col-name"><div class="sec-name">Transfer to such of certain persons as survive at some period not specified</div></td>
          <td class="col-concept">Survivorship gift (unspecified time)</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest to accrue to such of certain persons as shall be surviving at some period</li>
              <li>Exact period NOT specified</li>
              <li>Goes to those alive when prior/intermediate interest ceases (unless contrary intention)</li>
            </ul>
          </td>
          <td class="col-expl expl">If property is left to "B and C or the survivor," and no specific date is given for who must survive, the rule is: whoever is alive when the prior interest (e.g. a life estate) ends, takes the property.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A transfers to B for life, then to C and D equally, or to the survivor. C dies during B's lifetime. D survives B. At B's death, the property passes entirely to D.</div></td>
          <td class="col-read"><div class="read-with">S. 23 — contingent on uncertain event</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="void key">
          <td class="col-sec"><span class="sec-badge">S. 25</span></td>
          <td class="col-name"><div class="sec-name">Conditional transfer</div><div><span class="tag tag-void">CONDITION FAILS</span></div></td>
          <td class="col-concept">When conditions in transfers are void</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest fails if condition for its creation is:</li>
              <li><strong>(1)</strong> Impossible of performance</li>
              <li><strong>(2)</strong> Forbidden by law</li>
              <li><strong>(3)</strong> Would defeat provisions of any law</li>
              <li><strong>(4)</strong> Fraudulent</li>
              <li><strong>(5)</strong> Injurious to person or property of another</li>
              <li><strong>(6)</strong> Immoral or opposed to public policy (court's view)</li>
            </ul>
          </td>
          <td class="col-expl expl">A transfer attached to an impossible, illegal, immoral, or fraudulent condition is void. The condition must be legal, possible, and moral for the interest to take effect. This mirrors the Contract Act's provisions on void agreements.</td>
          <td class="col-illus"><div class="illus"><strong>Illustrations (from Act)</strong>(a) "Walk 100 miles in an hour" — impossible → void.<br>(b) Gift on condition of marrying A's daughter C, who was dead at transfer — impossible → void.<br>(c) Transfer Rs.500 to B if B murders C — illegal → void.<br>(d) Rs.500 to niece if she deserts her husband — immoral → void.</div></td>
          <td class="col-read"><div class="read-with">Indian Contract Act, S. 23, 56<br>S. 26 — condition precedent<br>S. 29 — condition subsequent</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 26</span></td>
          <td class="col-name"><div class="sec-name">Fulfilment of condition precedent</div></td>
          <td class="col-concept">Substantial compliance = fulfillment</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Condition to be fulfilled <em>before</em> taking the interest</li>
              <li>Deemed fulfilled if <strong>substantially complied with</strong></li>
            </ul>
          </td>
          <td class="col-expl expl">A condition that must be satisfied before the interest is enjoyed does not require perfect compliance — substantial performance is enough. Courts do not demand technical exactness for conditions precedent.</td>
          <td class="col-illus"><div class="illus"><strong>Illustrations (from Act)</strong>(a) Transfer to B on condition B marries with consent of C, D, and E. E dies. B marries with C and D's consent = condition fulfilled (substantially complied with).<br>(b) B marries without consent of C, D, E but obtains it after = condition NOT fulfilled.</div></td>
          <td class="col-read"><div class="read-with">S. 25 — conditional transfer<br>S. 29 — condition subsequent (strict fulfillment)</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 27</span></td>
          <td class="col-name"><div class="sec-name">Conditional transfer to one person coupled with transfer to another on failure of prior disposition</div></td>
          <td class="col-concept">Ulterior disposition on failure of prior</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest created for A; by same transaction, if prior fails, then to B</li>
              <li>Prior disposition fails <em>for any reason</em> → ulterior takes effect</li>
              <li><strong>Exception:</strong> if parties intended ulterior only on failure in a <em>particular manner</em>, it takes effect only on failure in that manner</li>
            </ul>
          </td>
          <td class="col-expl expl">If A's gift fails for any reason, B gets it — even if A failed in an unexpected way. But if the intent was that B only gets it if A fails in a specific way, then B only gets it if A actually fails that way.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>(a) Transfer to B; if B fails to execute a lease within 3 months of A's death, then to C. B dies in A's lifetime — B fails (but not in the specified manner). C's interest still takes effect.<br>(b) Transfer to wife, then to B if wife dies in A's lifetime. Both die simultaneously — it cannot be proved she died before him. B's disposition does NOT take effect.</div></td>
          <td class="col-read"><div class="read-with">S. 25 — conditional transfer<br>S. 28 — ulterior conditional transfer<br>S. 30 — invalidity of ulterior does not affect prior</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 28</span></td>
          <td class="col-name"><div class="sec-name">Ulterior transfer conditional on happening or not happening of specified event</div></td>
          <td class="col-concept">Conditional transfer with superadded condition</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest created for A, with condition: if uncertain event happens (or doesn't happen), it passes to B</li>
              <li>Subject to rules in Ss. 10, 12, 21, 22, 23, 24, 25, 27</li>
            </ul>
          </td>
          <td class="col-expl expl">You can create a gift with a condition attached — the property goes to A unless a specified event occurs, in which case it goes to B. The entire transfer is subject to the rules on valid conditions.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>Property to B, but if B goes to London within 2 years, then to C. This is a transfer with a superadded condition — B holds the property, but if the condition is triggered, C takes it.</div></td>
          <td class="col-read"><div class="read-with">S. 25, 27, 29 — related condition rules<br>S. 31 — condition making interest cease</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 29</span></td>
          <td class="col-name"><div class="sec-name">Fulfilment of condition subsequent</div></td>
          <td class="col-concept">Strict fulfillment for condition subsequent</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Ulterior disposition (under S.28) cannot take effect unless condition is <strong>strictly fulfilled</strong></li>
            </ul>
          </td>
          <td class="col-expl expl">Unlike condition precedent (S.26 — substantial compliance), a condition subsequent must be strictly performed to trigger the change of ownership. This protects the existing interest-holder.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>Transfer to B; if B dies a minor OR marries without C's consent, then to D. B marries at 17 without C's consent. Condition is strictly fulfilled — transfer to D takes effect.</div></td>
          <td class="col-read"><div class="read-with">S. 26 — condition precedent (substantial compliance)<br>S. 28 — ulterior transfer</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 30</span></td>
          <td class="col-name"><div class="sec-name">Prior disposition not affected by invalidity of ulterior disposition</div></td>
          <td class="col-concept">Invalid ulterior does not taint prior</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>If ulterior (subsequent) disposition is invalid</li>
              <li>Prior disposition is NOT affected — stands on its own</li>
            </ul>
          </td>
          <td class="col-expl expl">If the fallback gift is void (e.g. immoral condition), the original gift still stands. The invalidity of a subsequent condition does not corrupt the main gift.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>Farm to B for life; if she does not desert her husband, then to C. The condition (desertion) is immoral — ulterior disposition is void. B is entitled to the farm for life as if no condition existed.</div></td>
          <td class="col-read"><div class="read-with">S. 25 — void conditions<br>S. 27, S. 28 — ulterior dispositions</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 31</span></td>
          <td class="col-name"><div class="sec-name">Condition that transfer shall cease to have effect in case specified uncertain event happens or does not happen</div></td>
          <td class="col-concept">Defeasance condition</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest created, with condition: shall <em>cease</em> on happening/non-happening of an uncertain event</li>
              <li>Subject to S.12 (insolvency/alienation conditions)</li>
            </ul>
          </td>
          <td class="col-expl expl">A transfer can be made "defeasible" — it takes effect now, but can be defeated if a specified event occurs (or fails to occur). When the condition is triggered, the interest ends.</td>
          <td class="col-illus"><div class="illus"><strong>Illustrations (from Act)</strong>(a) Farm to B for life; if B cuts the wood, transfer ceases. B cuts the wood — loses life-interest.<br>(b) Farm to B; if B doesn't go to England within 3 years, interest ceases. B doesn't go — interest ceases.</div></td>
          <td class="col-read"><div class="read-with">S. 32 — condition must be valid<br>S. 12 — insolvency condition (void)</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 32</span></td>
          <td class="col-name"><div class="sec-name">Such condition must not be invalid</div></td>
          <td class="col-concept">Validity of defeasance condition</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Condition for interest to cease (S.31) must be valid</li>
              <li>The event must be one that could legally constitute the condition for <em>creation</em> of an interest</li>
            </ul>
          </td>
          <td class="col-expl expl">A defeasance condition (causing an interest to cease) must be as legally valid as a condition for creating an interest. If the event would be invalid as a condition precedent (e.g. immoral), it is equally invalid as a defeasance condition.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>Transfer to B; interest ceases if B does not commit fraud. This is void — fraud cannot legally be a condition for creating an interest, so it equally cannot be a defeasance condition.</div></td>
          <td class="col-read"><div class="read-with">S. 25 — conditions in creation<br>S. 31 — defeasance condition</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 33</span></td>
          <td class="col-name"><div class="sec-name">Transfer conditional on performance of act, no time being specified for performance</div></td>
          <td class="col-concept">Condition broken when performance rendered impossible</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest created subject to performing an act</li>
              <li>No time specified for performance</li>
              <li>Condition broken when transferee <em>renders performance impossible</em>, permanently or for indefinite period</li>
            </ul>
          </td>
          <td class="col-expl expl">If the condition is to do something and no deadline is set, the condition is only broken when the person makes it impossible to ever do that act. Mere delay is not a breach.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>Transfer to B if B builds a road on the land. No time is set. B paves the road path with permanent concrete buildings — rendering road-building permanently impossible. Condition is now broken.</div></td>
          <td class="col-read"><div class="read-with">S. 34 — when time is specified<br>S. 25 — conditional transfer</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 34</span></td>
          <td class="col-name"><div class="sec-name">Transfer conditional on performance of act, time being specified</div></td>
          <td class="col-concept">Fraud extends time; prevents benefit from own wrong</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Act to be performed within a specified time</li>
              <li>If performance is <em>prevented by fraud</em> of a person who benefits from non-fulfilment</li>
              <li>Extra time is allowed (against that fraudulent person) to make up for the delay</li>
              <li>If no time specified: if fraud renders performance impossible/indefinitely postponed → condition deemed fulfilled against that person</li>
            </ul>
          </td>
          <td class="col-expl expl">A person cannot benefit from their own fraudulent obstruction of a condition. If you fraudulently prevent the other party from meeting the condition, the law treats the condition as met — against you. No one can take advantage of their own wrong.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>Transfer to B if B builds a road within 2 years. C (who would benefit if B fails) secretly prevents delivery of building materials for 6 months. B is allowed 6 additional months as against C.</div></td>
          <td class="col-read"><div class="read-with">S. 33 — no time specified<br>Indian Contract Act, S. 53 (prevention of performance)</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 35</span></td>
          <td class="col-name"><div class="sec-name">Election when necessary</div><div><span class="tag tag-key">DOCTRINE</span></div></td>
          <td class="col-concept">Doctrine of election</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Person A professes to transfer property he has no right to (belongs to C)</li>
              <li>Same transaction confers a benefit on C</li>
              <li>C must elect: (1) confirm the transfer and take the benefit, OR (2) dissent — but must then relinquish the benefit</li>
              <li>If C enjoys the benefit for <strong>2 years</strong> without dissent = presumed to confirm</li>
              <li>If disability: election postponed until disability ends</li>
              <li>Where benefit is expressed "in lieu of" the property — C claiming property must give up that specific benefit (but not other benefits)</li>
            </ul>
          </td>
          <td class="col-expl expl">You cannot "approbate and reprobate" — you cannot take the good parts of a transaction and reject the bad. If you take the benefit given to you by a transaction, you are bound by the whole transaction. Choose one or the other.</td>
          <td class="col-illus"><div class="illus"><strong>Illustrations (from Act)</strong>A gifts C's farm (worth Rs.800) to B, and gives C Rs.1,000. C must elect: keep the farm (and lose Rs.1,000) OR give up the farm and get Rs.1,000. If C keeps the farm, Rs.1,000 is forfeited.<br><br>If A dies before C elects: A's estate must pay B Rs.800 from the Rs.1,000.</div></td>
          <td class="col-read"><div class="read-with">S. 6(a) — spes successionis<br>Indian Contract Act (consent)</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 36</span></td>
          <td class="col-name"><div class="sec-name">Apportionment of periodical payments on determination of interest of person entitled</div></td>
          <td class="col-concept">Apportionment of rents/income</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Rents, annuities, pensions, dividends, other periodical income</li>
              <li>On transfer of the interest: accrue from day to day</li>
              <li>Apportioned between transferor and transferee accordingly</li>
              <li>But payable on days appointed for payment</li>
              <li>Unless contrary contract or local usage</li>
            </ul>
          </td>
          <td class="col-expl expl">When a property that earns rent is transferred mid-month/mid-year, the income is split fairly between the seller (for days owned before transfer) and buyer (for days after). The payment date does not shift — only the entitlement is divided.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A owns a house earning Rs.3,000/month rent. A sells to B on the 15th. For that month, A gets Rs.1,500 (15 days), B gets Rs.1,500 — even though rent is paid on the 1st of next month.</div></td>
          <td class="col-read"><div class="read-with">S. 37 — apportionment of obligations<br>S. 55(1)(g) — seller pays charges to date of sale</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 37</span></td>
          <td class="col-name"><div class="sec-name">Apportionment of benefit of obligation on severance</div></td>
          <td class="col-concept">Apportionment of obligations on partition</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Property divided and held in several shares after transfer</li>
              <li>Obligation relating to property as a whole passes to several owners</li>
              <li>Each owner's share of obligation = proportionate to value of their share</li>
              <li>Condition: duty can be severed AND severance does not substantially increase the burden</li>
              <li>If duty cannot be severed: all owners jointly designate one person to perform it</li>
              <li>Obligation-holder not liable until given <em>reasonable notice</em> of severance</li>
              <li>Does NOT apply to agricultural leases (unless State Government notifies)</li>
            </ul>
          </td>
          <td class="col-expl expl">When one property is split among multiple buyers, the duties attached to it (like paying rent to a tenant) are split proportionally. But if splitting the duty would make it harder to perform, all owners must together decide who handles it.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A sells house leased to E (rent Rs.30/year) to B (½), C (¼), D (¼). E must pay B Rs.15, C Rs.7.50, D Rs.7.50 — and deliver one fat sheep jointly to all three.</div></td>
          <td class="col-read"><div class="read-with">S. 36 — apportionment of income<br>S. 44 — transfer by co-owner</div></td>
        </tr>

        <!-- Part B: Transfer of Immoveable Property -->
        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 38</span></td>
          <td class="col-name"><div class="sec-name">Transfer by person authorised only under certain circumstances to transfer</div></td>
          <td class="col-concept">Good faith transferee protected</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Person authorised to transfer only under <em>variable circumstances</em></li>
              <li>Alleges those circumstances exist</li>
              <li>Transferee uses <strong>reasonable care</strong> to ascertain existence of circumstances</li>
              <li>Transferee acts in <strong>good faith</strong></li>
              <li>Result: circumstances deemed to have existed (as between transferee and transferor/affected parties)</li>
            </ul>
          </td>
          <td class="col-expl expl">If someone can only sell under specific conditions (e.g. Hindu widow selling for legal necessity), and the buyer diligently checks and is satisfied those conditions exist, the buyer is protected even if it later turns out the conditions didn't fully exist.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>Hindu widow A claims her property income is insufficient for maintenance and sells a field to B. B does reasonable enquiry, satisfied necessity exists, buys in good faith. As between B and A/collateral heirs, necessity is deemed to have existed.</div></td>
          <td class="col-read"><div class="read-with">S. 41 — ostensible owner<br>S. 3 — notice</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 39</span></td>
          <td class="col-name"><div class="sec-name">Transfer where third person is entitled to maintenance</div></td>
          <td class="col-concept">Maintenance right enforceable against transferee with notice</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Third person has right to maintenance/advancement/marriage provision from profits of immoveable property</li>
              <li>Property is transferred</li>
              <li>Right enforceable against transferee if: (a) transferee had <strong>notice</strong>, OR (b) transfer is <strong>gratuitous</strong></li>
              <li>NOT enforceable against: transferee for consideration without notice</li>
            </ul>
          </td>
          <td class="col-expl expl">If a dependent has a maintenance right tied to the property, that right follows the property — but only if the new owner knew about it, or received the property as a gift. A genuine buyer without knowledge is protected.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>Property of A is charged with maintenance of A's sister C. A sells the property to B, who is told about C's right. B takes the property subject to C's maintenance claim.</div></td>
          <td class="col-read"><div class="read-with">S. 3 — notice<br>S. 40 — burden of obligation on land</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 40</span></td>
          <td class="col-name"><div class="sec-name">Burden of obligation imposing restriction on use of land or of obligation annexed to ownership but not amounting to interest or easement</div></td>
          <td class="col-concept">Restrictive covenants bind transferees with notice</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Third person has right to restrain enjoyment of another's land (independent of easement/interest), OR</li>
              <li>Third person entitled to benefit of obligation annexed to ownership (contractual, not easement)</li>
              <li>Right/obligation enforceable against: (a) transferee with <strong>notice</strong>, OR (b) gratuitous transferee</li>
              <li>NOT enforceable against: transferee for consideration without notice</li>
            </ul>
          </td>
          <td class="col-expl expl">A buyer who knows about a restriction on the land (e.g. a promise by the previous owner not to build above 2 floors) is bound by it. A buyer without notice who paid value is free of it. This is the foundation of the doctrine of notice in property law.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A contracts to sell Sultanpur to B. While contract is in force, A sells to C, who has notice of B's contract. B can enforce the contract against C to the same extent as against A.</div></td>
          <td class="col-read"><div class="read-with">S. 3 — notice<br>S. 11 — restriction on enjoyment<br>S. 39 — maintenance right</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key doctrine">
          <td class="col-sec"><span class="sec-badge">S. 41</span></td>
          <td class="col-name"><div class="sec-name">Transfer by ostensible owner</div><div><span class="tag tag-doctrine">DOCTRINE OF OSTENSIBLE OWNER</span></div></td>
          <td class="col-concept">Transfer by apparent owner with true owner's consent</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Person is <strong>ostensible (apparent) owner</strong> with express/implied consent of the real owner</li>
              <li>Transfers property for <strong>consideration</strong></li>
              <li>Transferee takes <strong>reasonable care</strong> to ascertain transferor's power</li>
              <li>Transferee acts in <strong>good faith</strong></li>
              <li>Result: transfer NOT voidable on ground that transferor was not authorised</li>
            </ul>
          </td>
          <td class="col-expl expl">If the real owner allows someone else to appear as the owner, and a bona fide purchaser buys from that apparent owner, the real owner cannot later reclaim the property. The law protects honest buyers who relied on the apparent ownership — the real owner should not have created the false appearance.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A (real owner) allows B to register the property in B's name and behave as owner. C buys from B, making reasonable inquiry and acting in good faith. A cannot recover the property from C.</div></td>
          <td class="col-read"><div class="read-with">S. 3 — notice<br>S. 38 — authorised transfer<br>S. 43 — transfer by unauthorised person</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 42</span></td>
          <td class="col-name"><div class="sec-name">Transfer by person having authority to revoke former transfer</div></td>
          <td class="col-concept">Subsequent transfer operates as revocation</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Transferor has reserved power to revoke a prior transfer</li>
              <li>Subsequently transfers the property for consideration to another</li>
              <li>This subsequent transfer operates as a revocation of the former transfer (to the extent of the power)</li>
            </ul>
          </td>
          <td class="col-expl expl">If A gave property to B but retained the right to revoke, and A then sells to C, the sale to C automatically revokes B's interest to the extent allowed. C's purchase is treated as A exercising the revocation power.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A lets house to B, reserving power to revoke if (per a surveyor) B makes detrimental use. A subsequently lets the house to C — this operates as a revocation of B's lease, subject to the surveyor's opinion.</div></td>
          <td class="col-read"><div class="read-with">S. 41 — ostensible owner<br>S. 126 — revocation of gift</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key doctrine">
          <td class="col-sec"><span class="sec-badge">S. 43</span></td>
          <td class="col-name"><div class="sec-name">Transfer by unauthorised person who subsequently acquires interest in property transferred</div><div><span class="tag tag-doctrine">FEEDING THE GRANT / ESTOPPEL</span></div></td>
          <td class="col-concept">Doctrine of feeding the grant by estoppel</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Person <strong>fraudulently or erroneously</strong> represents they are authorised to transfer immoveable property</li>
              <li>Transfers for <strong>consideration</strong></li>
              <li>Subsequently <strong>acquires</strong> that interest in the property</li>
              <li>At transferee's option: transfer operates on the newly acquired interest</li>
              <li>Contract of transfer must still be subsisting</li>
              <li>Does NOT affect a transferee for consideration without notice of this option</li>
            </ul>
          </td>
          <td class="col-expl expl">If someone sells you something they don't own yet, but later they acquire ownership, the earlier sale automatically "feeds" and becomes valid (at the buyer's option). The seller is estopped from denying the transfer. The buyer's earlier "bad" purchase is healed when the seller gets title.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A (Hindu, separated from father B) sells fields X, Y, Z to C. Z actually belongs to B. B dies; A inherits Z. C (who hasn't rescinded) may require A to deliver Z — the earlier transfer is fed by A's newly acquired title.</div></td>
          <td class="col-read"><div class="read-with">S. 41 — ostensible owner<br>S. 7 — competency to transfer</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 44</span></td>
          <td class="col-name"><div class="sec-name">Transfer by one co-owner</div></td>
          <td class="col-concept">Co-owner's transfer of their share</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Co-owner legally competent transfers their share or interest</li>
              <li>Transferee gets: transferor's right to joint possession, right to enforce partition</li>
              <li>Subject to conditions/liabilities on the share at date of transfer</li>
              <li><strong>Exception:</strong> if transferee of dwelling-house is NOT a family member of an undivided family — no right to joint possession</li>
            </ul>
          </td>
          <td class="col-expl expl">A co-owner can sell their own share — but the buyer only gets what the co-owner had. The buyer can ask for partition to get their specific portion. However, if it is a family home and the buyer is an outsider, they cannot barge in and demand to live there.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A, B, and C jointly own a house. A sells his 1/3 share to X (an outsider). X gets A's share and can demand partition — but cannot demand to live in the house until partition happens.</div></td>
          <td class="col-read"><div class="read-with">S. 37 — apportionment on severance<br>S. 47 — co-owners transferring common property share</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 45</span></td>
          <td class="col-name"><div class="sec-name">Joint transfer for consideration</div></td>
          <td class="col-concept">Proportionate interest in joint purchase</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Immoveable property transferred to 2+ persons</li>
              <li>Consideration from common fund: interests proportionate to their interests in the fund</li>
              <li>Consideration from separate funds: interests proportionate to their respective contributions</li>
              <li>If evidence is absent: presumed equal interests</li>
            </ul>
          </td>
          <td class="col-expl expl">When two people jointly buy property, their shares depend on how they paid. If they paid from a shared fund — their shares match their interest in that fund. If each paid separately — shares match their contributions.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A and B jointly buy a house for Rs.1,00,000. A pays Rs.60,000 from his own pocket; B pays Rs.40,000. A gets a 3/5 share; B gets 2/5 share.</div></td>
          <td class="col-read"><div class="read-with">S. 44 — co-owner's transfer<br>S. 46 — distinct interests</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 46</span></td>
          <td class="col-name"><div class="sec-name">Transfer for consideration by persons having distinct interests</div></td>
          <td class="col-concept">Proportionate share of consideration on joint sale</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Immoveable property transferred by persons having distinct interests</li>
              <li>Equal interests → share consideration equally</li>
              <li>Unequal interests → share consideration proportionately to value of interests</li>
              <li>Unless contrary contract</li>
            </ul>
          </td>
          <td class="col-expl expl">When multiple owners with different-sized interests sell together, the sale price is split in proportion to their interests. The person with a bigger share gets more of the money.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A (life interest worth Rs.600) and B, C (reversion worth Rs.400 total) sell mauza for Rs.1,000. A gets Rs.600; B and C together get Rs.400.</div></td>
          <td class="col-read"><div class="read-with">S. 45 — joint purchase<br>S. 47 — co-owners transferring a share</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 47</span></td>
          <td class="col-name"><div class="sec-name">Transfer by co-owners of share in common property</div></td>
          <td class="col-concept">Share transferred without specifying from whose portion</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Several co-owners transfer a share without specifying from which co-owner's share</li>
              <li>Transfer takes effect on each co-owner's share equally (if equal) or proportionately (if unequal)</li>
            </ul>
          </td>
          <td class="col-expl expl">If co-owners jointly sell "a 2-anna share" without saying who contributes what, the burden of the transfer is distributed across all their shares in proportion to what each owns.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A (8-anna), B (4-anna), C (4-anna) jointly transfer 2 annas to D without specifying. A contributes 1 anna, B contributes ½ anna, C contributes ½ anna — proportionally.</div></td>
          <td class="col-read"><div class="read-with">S. 44, S. 45, S. 46</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 48</span></td>
          <td class="col-name"><div class="sec-name">Priority of rights created by transfer</div></td>
          <td class="col-concept">Earlier right prevails (nemo dat)</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Person purports to create rights over same immoveable property at different times</li>
              <li>Rights cannot all exist to full extent together</li>
              <li>Earlier created right prevails (in absence of special contract/reservation binding earlier transferee)</li>
            </ul>
          </td>
          <td class="col-expl expl">You cannot give the same right twice. The first transfer prevails; subsequent transfers are subject to the first. This embodies the Latin maxim "nemo dat quod non habet" — you cannot give what you do not have.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages his land to B. Later, A tries to mortgage the same land to C. C's mortgage is subject to B's earlier mortgage.</div></td>
          <td class="col-read"><div class="read-with">S. 78, S. 79 — priority of mortgages<br>S. 3 — notice</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 49</span></td>
          <td class="col-name"><div class="sec-name">Transferee's right under policy</div></td>
          <td class="col-concept">Insurance money to be used for reinstatement</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Immoveable property transferred for consideration</li>
              <li>Property was insured against fire at date of transfer</li>
              <li>If property is destroyed/damaged by fire: transferee can require insurance money received by transferor to be applied in reinstating the property</li>
              <li>Unless contrary contract</li>
            </ul>
          </td>
          <td class="col-expl expl">If the seller had fire insurance on the property and the property burns down after sale (but before the insurance is sorted), the buyer can require the insurance payout to go towards rebuilding — not into the seller's pocket.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A sells insured shop to B. Before B takes full possession, the shop burns down. A receives Rs.5 lakh from insurance. B can require that money to be used to reinstate the shop.</div></td>
          <td class="col-read"><div class="read-with">S. 55 — rights of buyer/seller</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 50</span></td>
          <td class="col-name"><div class="sec-name">Rent bona fide paid to holder under defective title</div></td>
          <td class="col-concept">Good faith tenant protected</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Person holds immoveable property under a person with defective title</li>
              <li>In good faith pays rent to that person</li>
              <li>Later it appears that person had no right to receive rent</li>
              <li>Result: the payer is NOT chargeable again for that rent</li>
            </ul>
          </td>
          <td class="col-expl expl">A tenant who honestly pays rent to who they believed was the landlord is protected. They cannot be made to pay the same rent again to the real owner, as long as they acted in good faith.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A lets a field to B at Rs.50 rent, then transfers the field to C. B (not knowing of the transfer) pays rent to A in good faith. B is not chargeable with the rent so paid — B does not owe C that amount again.</div></td>
          <td class="col-read"><div class="read-with">S. 55(5)(a) — buyer's duty to disclose<br>S. 3 — notice</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 51</span></td>
          <td class="col-name"><div class="sec-name">Improvements made by bona fide holders under defective titles</div></td>
          <td class="col-concept">Good faith improver entitled to compensation</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Transferee in good faith believes they are absolutely entitled to property</li>
              <li>Makes improvements to the property</li>
              <li>Subsequently evicted by a person with better title</li>
              <li>Rights: require (a) value of improvement to be paid/secured, OR (b) sell their interest at market value (excluding improvement value)</li>
              <li>Improvement value assessed at time of eviction</li>
              <li>If crops growing at eviction: entitled to crops + free ingress/egress to gather</li>
            </ul>
          </td>
          <td class="col-expl expl">If you genuinely (though mistakenly) thought you owned the property and improved it, you should not lose those improvements for free when the real owner takes back. You are compensated for what you added.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B buys land from A in good faith (A had defective title). B builds a Rs.5 lakh house. C (real owner) evicts B. B can claim Rs.5 lakh for the house OR require C to sell his interest to B at market value.</div></td>
          <td class="col-read"><div class="read-with">S. 50 — good faith payment<br>S. 55(6)(a) — buyer's right to improvements</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key doctrine">
          <td class="col-sec"><span class="sec-badge">S. 52</span></td>
          <td class="col-name"><div class="sec-name">Transfer of property pending suit relating thereto</div><div><span class="tag tag-doctrine">LIS PENDENS</span></div></td>
          <td class="col-concept">Doctrine of lis pendens — transfer void as to suit parties</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Suit/proceeding in a competent court (not collusive)</li>
              <li>Any right to immoveable property directly and specifically in question</li>
              <li>During pendency: property cannot be transferred to affect rights of any party to the suit</li>
              <li>Exception: transfer with <strong>court authority</strong> on court's terms</li>
              <li>Pendency commences: date of plaint presentation / institution of proceeding</li>
              <li>Pendency ends: final decree + complete satisfaction/discharge, or limitation to execute expires</li>
            </ul>
          </td>
          <td class="col-expl expl">Once a court case is filed about the ownership of land, neither party can sell or transfer that land so as to defeat the other party's rights. Any such transfer is subject to whatever the court eventually decides. This prevents parties from selling the disputed property to defeat the litigation.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A files a suit against B for title to a plot. While the suit is pending, B sells the plot to C. C is bound by the outcome of A vs B — if A wins, C loses the property. C cannot claim to be an innocent purchaser who is free from the litigation.</div></td>
          <td class="col-read"><div class="read-with">S. 3 — notice<br>S. 41 — ostensible owner</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 53</span></td>
          <td class="col-name"><div class="sec-name">Fraudulent transfer</div><div><span class="tag tag-key">FRAUD</span></div></td>
          <td class="col-concept">Transfers to defraud creditors/subsequent transferees — voidable</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li><strong>Sub-section (1):</strong> Transfer with intent to <em>defeat or delay creditors</em> → voidable at creditor's option. Suit must be on behalf of ALL creditors. Protects bona fide transferee for consideration.</li>
              <li><strong>Sub-section (2):</strong> Transfer <em>without consideration</em> with intent to defraud a <em>subsequent transferee</em> → voidable at subsequent transferee's option. Transfer without consideration alone ≠ fraud.</li>
            </ul>
          </td>
          <td class="col-expl expl">If a debtor sells their property to hide it from creditors, those creditors can challenge the transfer in court. Similarly, if someone gives away property without payment specifically to cheat a later buyer, that later buyer can challenge it. But honest buyers who paid value are protected.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (sub-s.1)</strong>A owes Rs.10 lakh to multiple creditors. A gifts his house to his son to put it beyond creditors' reach. Creditors can challenge this as a fraudulent transfer — voidable at their option.<br><br><strong>Note:</strong> A genuine gift made without intent to defraud is not caught by sub-s. 2 merely because a later transfer for value was also made.</div></td>
          <td class="col-read"><div class="read-with">S. 53A — part performance<br>Indian Contract Act, S. 17 — fraud</div></td>
        </tr>

        <tr data-ch="ch2" data-tags="key doctrine">
          <td class="col-sec"><span class="sec-badge">S. 53A</span></td>
          <td class="col-name"><div class="sec-name">Part performance</div><div><span class="tag tag-doctrine">PART PERFORMANCE</span></div></td>
          <td class="col-concept">Doctrine of part performance — equity protects possessing transferee</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Contract to transfer immoveable property for consideration</li>
              <li>In <strong>writing signed</strong> by transferor (or on his behalf)</li>
              <li>Terms necessary to constitute the transfer are ascertainable with reasonable certainty</li>
              <li>Transferee has taken <strong>possession</strong> (or continues in possession) in part performance, AND done some act in furtherance, AND has performed or is <strong>willing to perform</strong> their part</li>
              <li>Effect: transferor debarred from enforcing any right against the transferee inconsistent with the contract</li>
              <li>Does NOT affect a transferee for consideration without notice of contract/part performance</li>
            </ul>
          </td>
          <td class="col-expl expl">This is an equity doctrine borrowed from English law. If you made a written contract to buy land, paid/are ready to pay, and are living on the land in part performance of the contract — the seller cannot kick you out just because the formal registration was not completed. Equity looks at substance over form.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A signs a written agreement to sell his farm to B for Rs.5 lakh. B pays Rs.2 lakh and takes possession, starts farming (act in furtherance). A then tries to evict B, claiming transfer incomplete (not registered). A is debarred — B is protected under S.53A.</div></td>
          <td class="col-read"><div class="read-with">S. 53 — fraudulent transfer<br>S. 54 — sale (registration)<br>Specific Relief Act — specific performance</div></td>
        </tr>

      </tbody>
    </table>
  </div>
</div>

<!-- ═══════════════════════════════════════════════════════ CHAPTER III -->
<div class="chapter-group ch3" id="grp-ch3">
  <div class="chapter-header" onclick="toggleChapter('ch3')">
    <span class="ch-roman">CHAPTER III</span>
    <span class="ch-title">Of Sales of Immoveable Property</span>
    <span class="ch-range">Sections 54–57</span>
    <span class="ch-toggle" id="tog-ch3">▼</span>
  </div>
  <div class="table-wrap" id="body-ch3">
    <table>
      <thead>
        <tr>
          <th class="col-sec">Section</th>
          <th class="col-name">Section Name (Bare Act)</th>
          <th class="col-concept">Concept</th>
          <th class="col-ingr">Ingredients / Requirements</th>
          <th class="col-expl">Simple Explanation</th>
          <th class="col-illus">Illustration</th>
          <th class="col-read">Read With</th>
        </tr>
      </thead>
      <tbody>

        <tr data-ch="ch3" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 54</span></td>
          <td class="col-name"><div class="sec-name">"Sale" defined. Sale how made. Contract for sale.</div><div><span class="tag tag-key">DEFINITION</span></div></td>
          <td class="col-concept">Definition of sale; mode of sale; contract for sale</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li><strong>Sale</strong> = transfer of ownership for a price paid/promised/part-paid and part-promised</li>
              <li><strong>Tangible immoveable ≥ Rs.100</strong> OR intangible (reversion etc.): registered instrument only</li>
              <li><strong>Tangible immoveable &lt; Rs.100:</strong> registered instrument OR delivery</li>
              <li><strong>Contract for sale:</strong> contract that a sale shall take place on terms settled — does NOT of itself create any interest in or charge on property</li>
            </ul>
          </td>
          <td class="col-expl expl">Sale is the outright transfer of ownership for money. It is final and permanent (unlike mortgage or lease). The mode depends on the value and nature of the property. A mere agreement to sell later is NOT a sale — it creates no property right yet.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A agrees in writing to sell his house to B for Rs.50 lakh in 3 months. This is only a contract for sale — B has no interest in the house yet. If A sells to C before the 3 months, B's remedy is a suit for specific performance, not a claim to the property itself (unless S.53A applies).</div></td>
          <td class="col-read"><div class="read-with">S. 53A — part performance<br>S. 55 — rights/liabilities<br>Indian Registration Act, 1908<br>S. 4 — supplemental to Registration Act</div></td>
        </tr>

        <tr data-ch="ch3" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 55</span></td>
          <td class="col-name"><div class="sec-name">Rights and liabilities of buyer and seller</div><div><span class="tag tag-key">KEY SECTION</span></div></td>
          <td class="col-concept">Mutual rights and duties in a sale</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li><strong>Seller bound to:</strong> (a) disclose material defects in property/title; (b) produce title documents on request; (c) answer relevant questions; (d) execute proper conveyance on payment; (e) take care of property between contract and delivery; (f) give possession; (g) pay charges/rent to date of sale, discharge incumbrances</li>
              <li><strong>Seller entitled to:</strong> (4a) rents/profits till ownership passes; (4b) charge on property for unpaid purchase money (if ownership passed early)</li>
              <li><strong>Buyer bound to:</strong> (5a) disclose material facts increasing seller's interest value; (5b) pay purchase money; (5c) bear losses after ownership passes; (5d) pay public charges after ownership passes</li>
              <li><strong>Buyer entitled to:</strong> (6a) improvements/rents after ownership passes; (6b) charge on property for purchase money paid before delivery</li>
              <li>Omission to disclose = fraudulent</li>
            </ul>
          </td>
          <td class="col-expl expl">Both buyer and seller have duties to each other to act fairly. The seller must be honest about defects; the buyer must be honest about facts that increase value. "Caveat emptor" (buyer beware) is modified — the seller cannot hide known defects.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (5a — buyer's duty)</strong>B knows the government plans to build a metro station next to the land he is buying from A — information A does not have, which would triple the land's value. B must disclose this to A. Failure to disclose = fraud.<br><br><strong>Illustration (seller's charge — 4b)</strong>A sells house to B; B takes possession but pays only half the price. A has a charge on the house for the remaining amount, even in B's hands.</div></td>
          <td class="col-read"><div class="read-with">S. 54 — sale defined<br>S. 3 — notice<br>S. 8 — operation of transfer<br>Indian Contract Act, S. 17 (fraud)</div></td>
        </tr>

        <tr data-ch="ch3" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 56</span></td>
          <td class="col-name"><div class="sec-name">Marshalling by subsequent purchaser</div></td>
          <td class="col-concept">Buyer entitled to burden mortgage on unsold land first</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Owner of 2+ properties mortgages them to one person</li>
              <li>Then sells one or more of those properties to another person</li>
              <li>Buyer is entitled to have the mortgage-debt satisfied out of the property NOT sold to him first</li>
              <li>Provided: not prejudicing mortgagee's rights; not prejudicing any other person who acquired an interest for consideration</li>
              <li>Unless contrary contract</li>
            </ul>
          </td>
          <td class="col-expl expl">If a seller had two properties mortgaged, and sold one of them to you, you can insist that the mortgagee first enforces against the property that was NOT sold to you. The buyer's equity should not be prejudiced by a debt on both properties when only one is sold.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages Farm X and Farm Y to B. A then sells Farm X to C. C can require B to first enforce the mortgage against Farm Y (unsold) before touching Farm X.</div></td>
          <td class="col-read"><div class="read-with">S. 81 — marshalling of securities (mortgage)<br>S. 82 — contribution to mortgage debt</div></td>
        </tr>

        <tr data-ch="ch3" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 57</span></td>
          <td class="col-name"><div class="sec-name">Provision by Court for incumbrances and sale freed therefrom</div></td>
          <td class="col-concept">Court can free property from incumbrances on payment</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Immoveable property subject to an incumbrance (immediately payable or not) is sold</li>
              <li>Court may, on any party's application, direct payment of money into Court to cover the incumbrance</li>
              <li>Annual/monthly charges or capital on determinable interest: amount sufficient to keep down the charge from investment income</li>
              <li>Other capital charges: amount sufficient to meet incumbrance + interest</li>
              <li>Plus contingency reserve (up to 1/10 of original amount, unless Court orders more for special reasons)</li>
              <li>After notice to incumbrancer: Court may declare property free from incumbrance</li>
              <li>"Court" means High Court, District Court, or notified court</li>
            </ul>
          </td>
          <td class="col-expl expl">When a mortgaged/encumbered property is sold (by court or privately), the court can handle paying off the encumbrance from the sale proceeds and declare the property free. This allows a clean transfer to the buyer without the encumbrance following.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A's property (mortgaged to B for Rs.5 lakh) is being sold. On application, Court directs that Rs.5.5 lakh (including contingency) be deposited in court. Court declares property free from B's mortgage. B receives payment from court; buyer gets clean title.</div></td>
          <td class="col-read"><div class="read-with">S. 56 — marshalling<br>S. 82 — contribution to mortgage debt<br>Code of Civil Procedure, Order 34</div></td>
        </tr>

      </tbody>
    </table>
  </div>
</div>

<!-- ═══════════════════════════════════════════════════════ CHAPTER IV -->
<div class="chapter-group ch4" id="grp-ch4">
  <div class="chapter-header" onclick="toggleChapter('ch4')">
    <span class="ch-roman">CHAPTER IV</span>
    <span class="ch-title">Of Mortgages of Immoveable Property and Charges</span>
    <span class="ch-range">Sections 58–104</span>
    <span class="ch-toggle" id="tog-ch4">▼</span>
  </div>
  <div class="table-wrap" id="body-ch4">
    <table>
      <thead>
        <tr>
          <th class="col-sec">Section</th>
          <th class="col-name">Section Name (Bare Act)</th>
          <th class="col-concept">Concept</th>
          <th class="col-ingr">Ingredients / Requirements</th>
          <th class="col-expl">Simple Explanation</th>
          <th class="col-illus">Illustration</th>
          <th class="col-read">Read With</th>
        </tr>
      </thead>
      <tbody>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 58(a)</span></td>
          <td class="col-name"><div class="sec-name">"Mortgage", "mortgagor", "mortgagee", "mortgage-money" and "mortgage-deed" defined</div><div><span class="tag tag-key">DEFINITION</span></div></td>
          <td class="col-concept">Mortgage defined; parties named</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li><strong>Mortgage</strong> = transfer of an interest in specific immoveable property to secure: (a) loan advanced or to be advanced, OR (b) existing or future debt, OR (c) performance of engagement that may give rise to pecuniary liability</li>
              <li><strong>Mortgagor:</strong> the transferor</li>
              <li><strong>Mortgagee:</strong> the transferee</li>
              <li><strong>Mortgage-money:</strong> principal + interest</li>
              <li><strong>Mortgage-deed:</strong> instrument (if any) effecting the transfer</li>
            </ul>
          </td>
          <td class="col-expl expl">A mortgage is NOT a sale. Only an "interest" transfers (not ownership) and it is for security purposes only. Once the debt is repaid, the mortgagor gets back everything. The distinguishing feature is the <em>purpose</em>: securing a debt.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A borrows Rs.10 lakh from B and transfers an "interest" in his house to B as security. A remains the owner; B holds an interest only until repayment. This is a mortgage, not a sale.</div></td>
          <td class="col-read"><div class="read-with">S. 59 — registration<br>S. 60 — right to redeem<br>S. 100 — charges</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 58(b)</span></td>
          <td class="col-name"><div class="sec-name">Simple mortgage</div></td>
          <td class="col-concept">Type 1 of 6: personal liability + right of sale</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>No delivery of possession</li>
              <li>Mortgagor <strong>binds himself personally</strong> to pay</li>
              <li>On default: mortgagee can cause property to be sold</li>
              <li>Proceeds applied to mortgage money</li>
            </ul>
          </td>
          <td class="col-expl expl">The borrower keeps the property, keeps possession, but personally promises to pay. If they default, the lender can get a court order to sell the property and recover the debt from sale proceeds. The mortgagee does NOT get the property directly — only sale proceeds.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A takes a home loan from B (bank). A keeps living in the house. If A defaults, B can apply to court to sell the house and recover the loan. A is also personally liable for any shortfall.</div></td>
          <td class="col-read"><div class="read-with">S. 67 — right to sale<br>S. 68 — right to sue for mortgage money<br>S. 96 — provisions apply to equitable mortgage</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 58(c)</span></td>
          <td class="col-name"><div class="sec-name">Mortgage by conditional sale</div></td>
          <td class="col-concept">Type 2 of 6: ostensible sale with redemption right</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagor ostensibly sells the property with one of these conditions:</li>
              <li>(i) On default of payment on certain date → sale becomes absolute, OR</li>
              <li>(ii) On payment → sale becomes void, OR</li>
              <li>(iii) On payment → buyer re-transfers to seller</li>
              <li><strong>Condition must be embodied in the same document</strong> as the sale (not a separate deed)</li>
            </ul>
          </td>
          <td class="col-expl expl">It looks like a sale but is actually a mortgage. The "buyer" knows they may have to give back the property if the "seller" repays. The condition making it a mortgage must be in the same document — if it is in a separate document, it is treated as an actual sale.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A executes a document "selling" his house to B for Rs.5 lakh, with a condition in the same document that if A repays Rs.5 lakh within 1 year, B will re-transfer the house. This is a mortgage by conditional sale — not a real sale.</div></td>
          <td class="col-read"><div class="read-with">S. 67 — only this mortgagee can foreclose<br>S. 58(a) — mortgage definition</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 58(d)</span></td>
          <td class="col-name"><div class="sec-name">Usufructuary mortgage</div></td>
          <td class="col-concept">Type 3 of 6: possession + rents to mortgagee</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagor delivers possession (or binds to deliver) to mortgagee</li>
              <li>Mortgagee authorised to retain possession until payment</li>
              <li>Mortgagee receives rents/profits — applied in lieu of interest, OR in payment of principal, OR both</li>
            </ul>
          </td>
          <td class="col-expl expl">The lender gets physical possession of the property and "uses" its income (rents/crops) to pay off the debt. The mortgagor does not pay cash interest; the property's income does the work. No personal liability to pay — the property pays for itself.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages his farm to B. B takes possession and takes the crop income (Rs.1 lakh/year). This goes towards interest and principal. Once the loan is paid off from accumulated income, B returns possession.</div></td>
          <td class="col-read"><div class="read-with">S. 62 — mortgagor's right to recover possession<br>S. 76 — mortgagee's liabilities in possession<br>S. 77 — receipts in lieu of interest</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 58(e)</span></td>
          <td class="col-name"><div class="sec-name">English mortgage</div></td>
          <td class="col-concept">Type 4 of 6: absolute transfer with personal covenant to repay</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagor binds to repay on a certain date</li>
              <li>Transfers the mortgaged property <strong>absolutely</strong> to the mortgagee</li>
              <li>Subject to a proviso: mortgagee will re-transfer on payment as agreed</li>
            </ul>
          </td>
          <td class="col-expl expl">The borrower technically transfers full ownership to the lender — but the lender promises to give it back on repayment. The lender has maximum security (they "own" the property), but is bound to reconvey on payment. Both personal liability AND property transfer exist.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A transfers his land to B absolutely, with a provision: if A pays Rs.10 lakh on 1 January next year, B will re-transfer the land. A is personally bound to pay; B holds the land as owner until payment.</div></td>
          <td class="col-read"><div class="read-with">S. 69 — power of sale without court (English mortgage)<br>S. 60 — right to redeem</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 58(f)</span></td>
          <td class="col-name"><div class="sec-name">Mortgage by deposit of title-deeds</div></td>
          <td class="col-concept">Type 5 of 6: equitable mortgage — deposit of documents</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Person in specified towns: Calcutta, Madras, Bombay (and State-notified towns)</li>
              <li>Delivers to creditor (or agent) documents of title to immoveable property</li>
              <li>With <strong>intent to create a security</strong> thereon</li>
              <li>No writing/registration needed</li>
            </ul>
          </td>
          <td class="col-expl expl">Just handing over your title documents (sale deed, etc.) to the bank with the intention of creating security creates a valid mortgage — without any written deed or registration. This is also called "equitable mortgage." Only available in specified towns.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A goes to his bank in Mumbai and deposits his flat's title documents (sale deed, etc.) as security for an overdraft. This creates a valid mortgage by deposit of title-deeds — no registration required.</div></td>
          <td class="col-read"><div class="read-with">S. 59 — registration NOT needed for this type<br>S. 96 — provisions of simple mortgage apply<br>S. 69(c) — power of sale in specified towns</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 58(g)</span></td>
          <td class="col-name"><div class="sec-name">Anomalous mortgage</div></td>
          <td class="col-concept">Type 6 of 6: any mortgage not fitting the 5 types above</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>A mortgage which is NOT: simple, conditional sale, usufructuary, English, or equitable (deposit of title-deeds)</li>
              <li>Governed by S. 98 — parties' contract + local usage</li>
            </ul>
          </td>
          <td class="col-expl expl">A residual category for mortgages that don't fit neatly into any of the five standard types. Could be a combination type or a locally evolved form. Its rights and liabilities are determined by the terms of the deed and local custom.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgage where the mortgagee takes possession AND also has the right to personal recovery — combining features of simple and usufructuary mortgage. This would be anomalous.</div></td>
          <td class="col-read"><div class="read-with">S. 98 — rights/liabilities of anomalous mortgage<br>S. 67 — anomalous mortgagee may foreclose if terms allow</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 59</span></td>
          <td class="col-name"><div class="sec-name">Mortgage when to be by assurance</div></td>
          <td class="col-concept">Registration requirement for mortgages</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Principal ≥ Rs.100 (other than mortgage by deposit of title-deeds): <strong>registered instrument</strong>, signed by mortgagor, attested by 2 witnesses</li>
              <li>Principal &lt; Rs.100: registered instrument OR (except simple mortgage) delivery of property</li>
              <li>Mortgage by deposit of title-deeds: <strong>NO registration required</strong></li>
            </ul>
          </td>
          <td class="col-expl expl">Most mortgages need to be formally registered. The exception is the equitable mortgage (deposit of title-deeds), which is created by the act of deposit itself. This makes equitable mortgages quicker and cheaper to create.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A creates a simple mortgage for Rs.5 lakh. It must be registered and attested by 2 witnesses. If A instead deposits his title deeds with the bank in Mumbai, no registration needed.</div></td>
          <td class="col-read"><div class="read-with">S. 58(f) — equitable mortgage<br>Indian Registration Act, 1908<br>S. 107 — leases (compare)</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 59A</span></td>
          <td class="col-name"><div class="sec-name">References to mortgagors and mortgagees to include persons deriving title from them</div></td>
          <td class="col-concept">Chapter IV applies to successors in title</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Unless otherwise expressly provided</li>
              <li>References to mortgagor/mortgagee include persons deriving title from them</li>
            </ul>
          </td>
          <td class="col-expl expl">The rights and duties in Chapter IV apply not just to the original mortgagor and mortgagee, but also to anyone who inherits or buys those positions (e.g. the mortgagor's legal heir, or a bank that bought out the mortgage). The mortgage follows the person/estate, not just the individual.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages property to B. A dies; property passes to A's son C. B dies; mortgage transferred to B's bank D. C can redeem from D; D can foreclose against C — S.59A ensures these rights continue.</div></td>
          <td class="col-read"><div class="read-with">S. 58 — mortgage defined<br>S. 60 — right to redeem</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 60</span></td>
          <td class="col-name"><div class="sec-name">Right of mortgagor to redeem. Redemption of portion of mortgaged property.</div><div><span class="tag tag-key">KEY RIGHT</span></div></td>
          <td class="col-concept">Right to redeem; "once a mortgage, always a mortgage"</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Arises: any time after principal money is <strong>due</strong></li>
              <li>On payment/tender of mortgage money, mortgagor can require mortgagee to: (a) return mortgage deed and related documents, (b) deliver possession (if held), (c) re-transfer property or acknowledge extinguishment</li>
              <li>Right continues until extinguished by <strong>act of parties</strong> or <strong>court decree</strong></li>
              <li>A suit to enforce this right = <strong>suit for redemption</strong></li>
              <li>Partial redemption: cannot redeem a share only (unless mortgagee acquired that co-mortgagor's share)</li>
            </ul>
          </td>
          <td class="col-expl expl">The right to get back your property by paying the debt is sacred and cannot be clogged. Any clause in the mortgage deed that says "you can never redeem" or makes redemption impossible/illusory is void. This principle is called "no clog on the equity of redemption."</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages house for 5 years. Clause in deed: "A shall never have the right to redeem." This clause is void — A can redeem at any time after the money is due by paying the full debt. No one can permanently block the mortgagor's right to redeem.</div></td>
          <td class="col-read"><div class="read-with">S. 83 — deposit in court<br>S. 91 — who can sue for redemption<br>S. 67 — mortgagee's right of foreclosure (extinguishes S.60)</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 60A</span></td>
          <td class="col-name"><div class="sec-name">Obligation to transfer to third party instead of re-transference to mortgagor</div></td>
          <td class="col-concept">Mortgagor can direct transfer to a third party</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagor entitled to redemption</li>
              <li>May require mortgagee to assign mortgage debt and property to a <strong>third party</strong> (instead of re-transfer to mortgagor)</li>
              <li>Mortgagee is bound to comply</li>
              <li>Rights of encumbrancers: prior encumbrancer's requisition prevails over mortgagor's; subsequent mortgagee's requisition prevails over mortgagor's</li>
              <li>Does NOT apply to mortgagee who is or has been in possession</li>
            </ul>
          </td>
          <td class="col-expl expl">On redeeming, the mortgagor doesn't have to take back the property himself — he can direct the mortgagee to transfer it directly to any third party he chooses (useful if selling immediately after redemption).</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages property to B. A redeems but is simultaneously selling to C. Instead of B→A and then A→C, A can require B to transfer directly to C under S.60A, saving time and registration costs.</div></td>
          <td class="col-read"><div class="read-with">S. 60 — right to redeem<br>S. 92 — subrogation</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 60B</span></td>
          <td class="col-name"><div class="sec-name">Right to inspection and production of documents</div></td>
          <td class="col-concept">Mortgagor's right to inspect documents</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagor's right of redemption must still subsist</li>
              <li>At all reasonable times, on request, at own cost (plus mortgagee's costs)</li>
              <li>Right to inspect and make copies/abstracts/extracts of title documents held by mortgagee</li>
            </ul>
          </td>
          <td class="col-expl expl">While the mortgage exists, the mortgagor has the right to see and copy their own title documents (which are held by the mortgagee as security). The mortgagor remains the owner and must have access to their documents for any other dealings.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A's title deed is held by bank B as security. A needs to verify a boundary dispute — A can request B to let him inspect and copy the title deed at A's cost.</div></td>
          <td class="col-read"><div class="read-with">S. 60 — right to redeem<br>S. 76(g) — mortgagee to keep accounts</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 61</span></td>
          <td class="col-name"><div class="sec-name">Right to redeem separately or simultaneously</div></td>
          <td class="col-concept">Multiple mortgages to same mortgagee — separate redemption allowed</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagor has executed 2+ mortgages to same mortgagee</li>
              <li>Principal of any 2+ mortgages has become due</li>
              <li>Can redeem any one separately OR two or more together</li>
              <li>Unless contrary contract</li>
            </ul>
          </td>
          <td class="col-expl expl">A borrower who has taken multiple loans from the same bank secured on different properties can choose to repay and redeem any one mortgage without being forced to clear all mortgages at once. This prevents "consolidation" — the bank forcing you to repay all or nothing.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A has 3 mortgages with Bank B (Property 1, 2, 3). A wants to redeem Property 1 only. Bank B cannot say "pay all 3 or none." A can redeem Property 1 independently.</div></td>
          <td class="col-read"><div class="read-with">S. 60 — right to redeem<br>S. 67A — mortgagee to sue on all mortgages (compare)</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 62</span></td>
          <td class="col-name"><div class="sec-name">Right of usufructuary mortgagor to recover possession</div></td>
          <td class="col-concept">Usufructuary mortgagor's right to get property back</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Usufructuary mortgage (mortgagee in possession, collecting income)</li>
              <li>If mortgagee authorised to pay mortgage money from rents/profits: mortgagor recovers possession when <strong>money is paid off</strong> from income</li>
              <li>If mortgagee authorised to collect only <em>part</em>: mortgagor recovers when the term expires AND mortgagor pays/tenders the balance</li>
            </ul>
          </td>
          <td class="col-expl expl">In a usufructuary mortgage, possession is given over. The mortgagor gets it back either when the debt is paid off entirely from the rental income, or when the mortgage period ends and the remaining balance is tendered.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A gives farm to B (usufructuary mortgagee) who collects Rs.50,000/year. Debt = Rs.2 lakh. After 4 years, when Rs.2 lakh is paid off from collections, A can recover the farm from B without paying anything.</div></td>
          <td class="col-read"><div class="read-with">S. 58(d) — usufructuary mortgage<br>S. 76 — mortgagee's liabilities in possession</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 63</span></td>
          <td class="col-name"><div class="sec-name">Accession to mortgaged property. Accession acquired in virtue of transferred ownership.</div></td>
          <td class="col-concept">Accretions to property benefit mortgagor on redemption</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagee in possession; property receives accession during mortgage</li>
              <li>On redemption: mortgagor entitled to the accession (unless contrary contract)</li>
              <li>If accession acquired at mortgagee's expense and is capable of <em>separate possession</em>: mortgagor must pay mortgagee's expense to take it</li>
              <li>If not separately possessible: delivered with the property; mortgagor pays proper cost (as addition to principal with 9% interest) if accession was necessary to preserve property OR made with mortgagor's assent</li>
              <li>Profits from accession: credited to mortgagor</li>
            </ul>
          </td>
          <td class="col-expl expl">If the property grows or is improved while the mortgagee holds it (e.g. alluvial soil deposits, or a new building), the mortgagor gets those accretions back on redemption. But if the mortgagee spent money on them, they are entitled to be reimbursed.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A's mortgaged field (held by B) gains new land by river alluvion. On redemption, A gets the enlarged field. If B had built a fence at his expense to protect the land and it cannot be removed, A pays B's cost of the fence as part of the mortgage money.</div></td>
          <td class="col-read"><div class="read-with">S. 63A — improvements<br>S. 70 — mortgagee's right to accession (compare)</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 63A</span></td>
          <td class="col-name"><div class="sec-name">Improvements to mortgaged property</div></td>
          <td class="col-concept">Improvements by mortgagee in possession — reimbursement</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagee in possession improves the property during mortgage</li>
              <li>On redemption: mortgagor entitled to the improvement; NOT liable to pay cost (generally)</li>
              <li><strong>Exception — mortgagor must pay</strong> if improvement: (a) necessary to prevent destruction/deterioration; (b) necessary to prevent security becoming insufficient; (c) made in compliance with lawful order of public authority</li>
              <li>In those cases: add proper cost to principal at same interest rate (or 9% p.a.)</li>
              <li>Profits from improvement credited to mortgagor</li>
            </ul>
          </td>
          <td class="col-expl expl">Mortgagees cannot charge for routine improvements they chose to make. But if they had to improve to save the property or comply with law, the mortgagor must reimburse them — those were genuinely necessary expenses, not voluntary upgrades.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B (mortgagee in possession) repaints the house at his own choice — Rs.50,000. On redemption, A (mortgagor) is NOT liable to pay for the paint job (voluntary improvement). But if B repaired a crumbling wall to prevent collapse (necessary), A must reimburse B.</div></td>
          <td class="col-read"><div class="read-with">S. 63 — accession to property<br>S. 72 — rights of mortgagee in possession</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 64</span></td>
          <td class="col-name"><div class="sec-name">Renewal of mortgaged lease</div></td>
          <td class="col-concept">Mortgagor benefits from lease renewal by mortgagee</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgaged property is a lease</li>
              <li>Mortgagee obtains a renewal of the lease</li>
              <li>On redemption: mortgagor has the benefit of the new lease (unless contrary contract)</li>
            </ul>
          </td>
          <td class="col-expl expl">If the mortgaged property is a lease, and the mortgagee (who holds it) renews that lease during the mortgage, the renewed lease belongs to the mortgagor on redemption — not the mortgagee personally. The mortgagee cannot use their position to grab a better lease for themselves.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages his 10-year leasehold flat (5 years remaining) to B. B renews the lease for 10 more years. When A redeems, A gets the benefit of the renewed 10-year lease.</div></td>
          <td class="col-read"><div class="read-with">S. 71 — mortgagee's right on renewal (mirror rule)<br>S. 62 — recovery of possession</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 65</span></td>
          <td class="col-name"><div class="sec-name">Implied contracts by mortgagor</div></td>
          <td class="col-concept">Mortgagor's implied promises to mortgagee</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Unless contrary contract, mortgagor is deemed to contract:</li>
              <li><strong>(a)</strong> Interest subsists; mortgagor has power to transfer</li>
              <li><strong>(b)</strong> Will defend (or enable mortgagee to defend) title</li>
              <li><strong>(c)</strong> Will pay public charges while not in mortgagee's possession</li>
              <li><strong>(d)</strong> If leasehold: rent and conditions paid/performed; will continue to pay and perform</li>
              <li><strong>(e)</strong> If subsequent mortgage: will pay interest on prior incumbrances; will discharge principal at proper time</li>
              <li>Benefit of these contracts goes to every person in whom mortgagee's interest vests</li>
            </ul>
          </td>
          <td class="col-expl expl">The law reads certain promises into every mortgage automatically, even if not written down. The mortgagor must protect the mortgagee's security — pay property taxes, defend title, keep up with any earlier loans. These are the basic duties that make security meaningful.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages his house to B without any written covenants. If government property tax falls due, A must pay it (S.65(c)). If someone else claims title to the house, A must defend B's security (S.65(b)).</div></td>
          <td class="col-read"><div class="read-with">S. 55(2) — seller's implied covenant on title<br>S. 66 — waste by mortgagor</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 65A</span></td>
          <td class="col-name"><div class="sec-name">Mortgagor's power to lease</div></td>
          <td class="col-concept">Mortgagor in possession can make binding leases</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagor in <strong>lawful possession</strong></li>
              <li>Can make leases binding on mortgagee, subject to:</li>
              <li>(a) Ordinary course of management; any local law/custom</li>
              <li>(b) Best rent; no premium; no advance rent</li>
              <li>(c) No covenant for renewal</li>
              <li>(d) Takes effect within 6 months of being made</li>
              <li>(e) Buildings: maximum lease duration = <strong>3 years</strong>; must contain rent covenant and re-entry clause</li>
              <li>Mortgage deed can vary/extend these limits</li>
            </ul>
          </td>
          <td class="col-expl expl">The mortgagor (who usually stays in possession) can continue renting out parts of the property during the mortgage — and those leases bind the mortgagee. But the leases must be commercially reasonable and short-term, to protect the mortgagee's security value.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A has mortgaged his building to B but remains in possession. A can rent out shops in the building for up to 3 years at market rent — these leases bind B. A cannot give a 10-year lease (exceeds 3-year limit for buildings) without B's consent.</div></td>
          <td class="col-read"><div class="read-with">S. 66 — waste by mortgagor<br>S. 105 — lease defined</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 66</span></td>
          <td class="col-name"><div class="sec-name">Waste by mortgagor in possession</div></td>
          <td class="col-concept">Mortgagor must not damage property if security insufficient</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagor in possession is NOT liable for allowing property to deteriorate (passive waste)</li>
              <li>BUT must NOT commit acts that are <strong>destructive or permanently injurious</strong></li>
              <li>This prohibition applies if: security is insufficient OR will be rendered insufficient by the act</li>
              <li><strong>Security is insufficient</strong> when property value does NOT exceed mortgage amount by: 1/3 (non-buildings) OR 1/2 (buildings)</li>
            </ul>
          </td>
          <td class="col-expl expl">The mortgagor can let normal wear and tear happen (no duty to maintain perfectly). But actively destroying the property — especially if the property's value barely covers the debt — is a breach. The mortgagee's security must not be deliberately destroyed.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages his house (worth Rs.10 lakh) for Rs.8 lakh. A demolishes one wing of the house (permanently injurious). The security is insufficient (building must exceed mortgage by ½ = Rs.12 lakh needed). A is in breach of S.66.</div></td>
          <td class="col-read"><div class="read-with">S. 65 — implied contracts by mortgagor<br>S. 72 — rights of mortgagee in possession</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 67</span></td>
          <td class="col-name"><div class="sec-name">Right to foreclosure or sale</div><div><span class="tag tag-key">KEY RIGHT</span></div></td>
          <td class="col-concept">Mortgagee's right of foreclosure or sale</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Arises: after mortgage money is due; before: (a) redemption decree; (b) payment/deposit of mortgage money</li>
              <li><strong>Foreclosure:</strong> mortgagor absolutely barred from redeeming → only available to: mortgagee by conditional sale, OR anomalous mortgagee entitled to foreclose by terms</li>
              <li><strong>Sale:</strong> court-ordered sale of property → available to all (except usufructuary mortgagee as such; mortgagee by conditional sale cannot also sue for sale)</li>
              <li>Cannot be used by: trustee/legal representative of mortgagor; mortgagee of public utilities (railway, canal etc.); partial interest holder without consent</li>
            </ul>
          </td>
          <td class="col-expl expl">Foreclosure is the nuclear option — it destroys the mortgagor's right to redeem permanently. It is only available to two types of mortgagees. All others must go for sale — which protects the mortgagor because any surplus from sale goes to them.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B (simple mortgagee) cannot foreclose — must sue for sale. C (mortgagee by conditional sale) can sue for foreclosure. Once a foreclosure decree is passed and made absolute, A (mortgagor) loses all right to the property.</div></td>
          <td class="col-read"><div class="read-with">S. 60 — right to redeem (extinguished on foreclosure)<br>S. 68 — right to sue for money<br>S. 69 — power of sale without court</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 67A</span></td>
          <td class="col-name"><div class="sec-name">Mortgagee when bound to bring one suit on several mortgages</div></td>
          <td class="col-concept">Mortgagee must sue on all due mortgages together</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagee holds 2+ mortgages by same mortgagor</li>
              <li>Has right to same kind of decree (S.67) on each</li>
              <li>Sues on one → must sue on all mortgages where money has become due</li>
              <li>Unless contrary contract</li>
            </ul>
          </td>
          <td class="col-expl expl">A lender who holds multiple mortgages from the same borrower cannot drip-feed lawsuits — one per mortgage, prolonging the mortgagor's agony. If you want to sue, sue for everything that has fallen due at once.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B holds mortgages on 3 properties of A, all with overdue principal. B sues to foreclose Mortgage 1 only. B is bound to include Mortgages 2 and 3 (where money is due) in the same suit.</div></td>
          <td class="col-read"><div class="read-with">S. 67 — right to foreclosure/sale<br>S. 61 — mortgagor's right to redeem separately</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 68</span></td>
          <td class="col-name"><div class="sec-name">Right to sue for mortgage-money</div></td>
          <td class="col-concept">When mortgagee can sue personally for the debt</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagee has right to sue for mortgage money ONLY in these cases:</li>
              <li><strong>(a)</strong> Mortgagor bound himself to repay (simple mortgage)</li>
              <li><strong>(b)</strong> Property destroyed/security insufficient (not mortgagor's or mortgagee's fault); mortgagee gave notice to provide further security; mortgagor failed</li>
              <li><strong>(c)</strong> Mortgagor's wrongful act/default deprives mortgagee of security</li>
              <li><strong>(d)</strong> Mortgagee entitled to possession; mortgagor fails to deliver or secure possession</li>
              <li>NOTE: in cases (a) and (b), court MAY stay the suit until mortgagee exhausts remedies against the property</li>
            </ul>
          </td>
          <td class="col-expl expl">A mortgagee's primary remedy is against the property, not the person. Only in specific circumstances can the lender sue the borrower personally for the debt. This protects borrowers from being pursued personally when the property remedy is adequate.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A's mortgaged factory (usufructuary) is destroyed by fire. B (mortgagee) cannot sue A personally — no personal liability in usufructuary mortgage. But under S.68(b), if B gave notice to provide more security and A refused, B may sue for the money.</div></td>
          <td class="col-read"><div class="read-with">S. 67 — foreclosure/sale<br>S. 69 — power of sale<br>S. 65(a) — implied contract of mortgagor</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 69</span></td>
          <td class="col-name"><div class="sec-name">Power of sale when valid</div><div><span class="tag tag-key">KEY POWER</span></div></td>
          <td class="col-concept">Mortgagee's power to sell without court</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Valid in three cases: (a) English mortgage — neither party Hindu/Muslim/Buddhist; (b) Mortgagee is Government + power expressly in deed; (c) Property in specified towns (Calcutta, Madras, Bombay, etc.) + power expressly in deed</li>
              <li><strong>Pre-conditions:</strong> (i) 3 months' written notice of default given + default continues; OR (ii) interest ≥ Rs.500 in arrear for 3 months</li>
              <li>Purchaser's title: not impeachable for irregularity in exercise of power; person damnified may sue in damages</li>
              <li>Proceeds: discharge prior incumbrances → costs of sale → mortgage money → surplus to mortgagor</li>
            </ul>
          </td>
          <td class="col-expl expl">Normally, selling mortgaged property requires going to court. In these three specific situations, the mortgagee can sell directly — saving time and cost. But notice must be given first. If the power is irregularly exercised, the buyer's title is still good, but the mortgagee can be sued for damages.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>Bank B holds an English mortgage on A's house (no Hindu/Muslim/Buddhist parties). A defaults for 4 months. B gives written notice. A still doesn't pay after 3 months of notice. B can now sell A's house directly without going to court under S.69.</div></td>
          <td class="col-read"><div class="read-with">S. 67 — foreclosure/court sale<br>S. 69A — appointment of receiver<br>S. 58(e) — English mortgage</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 69A</span></td>
          <td class="col-name"><div class="sec-name">Appointment of receiver</div></td>
          <td class="col-concept">Mortgagee can appoint a receiver to collect income</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagee who has power of sale under S.69 can appoint a receiver in writing</li>
              <li>Receiver is agent of mortgagor; mortgagor solely responsible for receiver's acts (unless mortgagee improperly intervened)</li>
              <li>Receiver may: demand/recover income, sue, give valid receipts</li>
              <li>Receiver's commission: max 5% of gross amounts received</li>
              <li>Receiver applies money in this order: (i) rents, taxes, outgoings; (ii) prior incumbrances' interest; (iii) receiver's commission + insurance premiums + repairs; (iv) mortgage interest; (v) if directed — principal; (vi) surplus to mortgagor</li>
              <li>Mortgagee can direct receiver to insure property</li>
            </ul>
          </td>
          <td class="col-expl expl">Instead of taking possession himself (with all its duties under S.76), the mortgagee can appoint a manager/receiver to collect rents from the property and apply them to the mortgage. The receiver is technically the mortgagor's agent, not the mortgagee's — protecting the mortgagee from liability for the receiver's defaults.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B (English mortgagee) appoints R as receiver for A's mortgaged commercial complex. R collects Rs.2 lakh/month rent, pays property tax, maintenance, receiver's fee, mortgage interest, and sends surplus to A. B never enters possession personally.</div></td>
          <td class="col-read"><div class="read-with">S. 69 — power of sale (prerequisite)<br>S. 76 — liabilities of mortgagee in possession (avoided by using receiver)</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 70</span></td>
          <td class="col-name"><div class="sec-name">Accession to mortgaged property</div></td>
          <td class="col-concept">Mortgagee's security extends to accretions</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>After date of mortgage, any accession is made to mortgaged property</li>
              <li>Mortgagee entitled to such accession for purposes of security</li>
              <li>Unless contrary contract</li>
            </ul>
          </td>
          <td class="col-expl expl">The mortgagee's security automatically extends to any additions to the property — new land by alluvion, a new building erected, etc. The mortgagor cannot argue that the addition is outside the mortgage.</td>
          <td class="col-illus"><div class="illus"><strong>Illustrations (from Act)</strong>(a) A mortgages field bordering a river to B. Field increases by alluvion (river deposits). B's security extends to the enlarged field.<br>(b) A mortgages a plot to B, then builds a house on it. B's security covers the house too.</div></td>
          <td class="col-read"><div class="read-with">S. 63 — mortgagor's accession right on redemption (compare)<br>S. 71 — renewal of mortgaged lease</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 71</span></td>
          <td class="col-name"><div class="sec-name">Renewal of mortgaged lease</div></td>
          <td class="col-concept">Mortgagor's renewal of lease benefits mortgagee</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgaged property is a lease</li>
              <li>Mortgagor obtains renewal of lease</li>
              <li>Mortgagee is entitled to the new lease for purposes of security (unless contrary contract)</li>
            </ul>
          </td>
          <td class="col-expl expl">The mirror of S.64 — just as S.64 protects the mortgagor when the mortgagee renews the lease, S.71 protects the mortgagee when the mortgagor renews. If the mortgagor renews the leasehold during the mortgage, the new lease also becomes part of the mortgagee's security.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages his 5-year leasehold flat to B. A renews the lease for 10 more years. B's mortgage automatically extends to cover the renewed 10-year lease period.</div></td>
          <td class="col-read"><div class="read-with">S. 64 — mortgagee's renewal (compare — benefits mortgagor)<br>S. 70 — accession to mortgaged property</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 72</span></td>
          <td class="col-name"><div class="sec-name">Rights of mortgagee in possession</div></td>
          <td class="col-concept">Mortgagee in possession can spend money and add to principal</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagee may spend necessary money for:</li>
              <li>(b) Preservation from destruction, forfeiture, or sale</li>
              <li>(c) Supporting mortgagor's title</li>
              <li>(d) Making own title good against mortgagor</li>
              <li>(e) Renewal of renewable leasehold</li>
              <li>Can add such money to principal (at same interest rate, or 9% p.a. default)</li>
              <li>Expenditure under (b) and (c) not "necessary" unless mortgagor was called upon and failed to act</li>
              <li>May also insure property against fire (up to 2/3 of reinstatement value); premiums added to principal</li>
              <li>Cannot insure if mortgagor already maintains sufficient insurance</li>
            </ul>
          </td>
          <td class="col-expl expl">A mortgagee who is in possession can protect their security by spending money on the property — and they get that money back (with interest) on top of the mortgage debt. They are permitted (but usually only after notifying the mortgagor) to spend to preserve the property.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B (mortgagee in possession) learns that the government will seize A's property for unpaid revenue. B pays the arrears (Rs.50,000) to prevent forfeiture. B can add this Rs.50,000 (with interest at 9% p.a.) to the mortgage money.</div></td>
          <td class="col-read"><div class="read-with">S. 76 — liabilities of mortgagee in possession<br>S. 63A — improvements by mortgagee</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 73</span></td>
          <td class="col-name"><div class="sec-name">Right to proceeds of revenue sale or compensation on acquisition</div></td>
          <td class="col-concept">Mortgagee's claim on compulsory sale/acquisition proceeds</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li><strong>Sub-s.(1) Revenue sale:</strong> property sold for arrears of revenue/charges and failure NOT due to mortgagee's default → mortgagee can claim mortgage money from surplus proceeds</li>
              <li><strong>Sub-s.(2) Acquisition:</strong> property acquired under Land Acquisition Act/other compulsory acquisition law → mortgagee can claim mortgage money from compensation amount due to mortgagor</li>
              <li><strong>Sub-s.(3):</strong> Claims prevail over all except prior encumbrances; enforceable even if principal not yet due</li>
            </ul>
          </td>
          <td class="col-expl expl">When the government compulsorily acquires the mortgaged property or it is sold for revenue default, the mortgagee's security does not evaporate. The mortgagee can step in and claim the mortgage debt from whatever compensation/proceeds are paid — ahead of other creditors (except prior encumbrancers).</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A's farm (mortgaged to B for Rs.5 lakh) is acquired by the government for a highway. The government pays Rs.10 lakh compensation to A. B can claim Rs.5 lakh (+ interest) from this compensation before A gets the rest.</div></td>
          <td class="col-read"><div class="read-with">S. 56 — marshalling (sale context)<br>Land Acquisition Act, 1894</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 74, 75</span></td>
          <td class="col-name"><div class="sec-name">[S.74 Right of subsequent mortgagee to pay off prior mortgagee] [S.75 Rights of mesne mortgagee] — Both Repealed</div></td>
          <td class="col-concept">Repealed sections</td>
          <td class="col-ingr"><span class="repealed">Both repealed by the Transfer of Property (Amendment) Act, 1929 (Act 20 of 1929), S.39. Now replaced by S.92 (subrogation) and S.94 (mesne mortgagee's rights) respectively.</span></td>
          <td class="col-expl expl"><span class="repealed">Replaced by improved provisions: S.92 covers subrogation (right of person who redeems to step into mortgagee's shoes); S.94 covers mesne mortgagee's rights against subsequent mortgagees.</span></td>
          <td class="col-illus"><div class="illus"><span class="repealed">Refer to S.92 and S.94 for the operative law.</span></div></td>
          <td class="col-read"><div class="read-with">S. 92 — subrogation<br>S. 94 — mesne mortgagee</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 76</span></td>
          <td class="col-name"><div class="sec-name">Liabilities of mortgagee in possession. Loss occasioned by his default.</div><div><span class="tag tag-key">KEY LIABILITIES</span></div></td>
          <td class="col-concept">Duties of mortgagee in possession — must manage prudently</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li><strong>(a)</strong> Manage as prudent owner of own property</li>
              <li><strong>(b)</strong> Use best endeavours to collect rents/profits</li>
              <li><strong>(c)</strong> Pay government revenue, public charges, and rent accruing due</li>
              <li><strong>(d)</strong> Make necessary repairs from rents/profits (after deducting charges and interest)</li>
              <li><strong>(e)</strong> Not commit destructive or permanently injurious acts</li>
              <li><strong>(f)</strong> Apply insurance money in reinstating property (or in mortgage reduction if mortgagor directs)</li>
              <li><strong>(g)</strong> Keep clear, full, accurate accounts; give copies to mortgagor on request</li>
              <li><strong>(h)</strong> Receipts from property (or fair occupation rent) credited against interest, then principal; surplus to mortgagor</li>
              <li><strong>(i)</strong> When mortgagor tenders/deposits due amount: must account for receipts from that date; cannot deduct post-tender expenses</li>
              <li>Failure in any duty → debited with resulting loss in accounts</li>
            </ul>
          </td>
          <td class="col-expl expl">A mortgagee who takes possession must manage the property like a responsible owner. They cannot milk the property or mismanage it. All income must be accounted for and applied against the debt — any surplus eventually goes back to the mortgagor. Poor management is penalised in the accounts.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B (mortgagee in possession) neglects to find tenants for 2 years despite market demand. B is debited for 2 years of rental income he could have collected but didn't (S.76(b) — best endeavours to collect).</div></td>
          <td class="col-read"><div class="read-with">S. 72 — rights of mortgagee in possession<br>S. 77 — receipts in lieu of interest<br>S. 63 — accession<br>S. 66 — waste by mortgagor (compare)</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 77</span></td>
          <td class="col-name"><div class="sec-name">Receipts in lieu of interest</div></td>
          <td class="col-concept">Contract to accept income as interest — exempts mortgagee from some duties</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>If there is a contract: receipts from mortgaged property taken <em>in lieu of interest</em> (or as part-interest and part-principal)</li>
              <li>Then: clauses (b), (d), (g), (h) of S.76 do NOT apply</li>
            </ul>
          </td>
          <td class="col-expl expl">If the mortgage deed says "B takes all rental income instead of charging interest," then B is not required to account in the detailed way S.76 normally demands for those specific items. The parties have contracted out of the usual accounting obligations.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages farmland to B; deed says B keeps all crop income in lieu of interest (no separate interest payment). S.76(b)(d)(g)(h) do not apply — B keeps the income without detailed accounting under those clauses.</div></td>
          <td class="col-read"><div class="read-with">S. 76 — liabilities of mortgagee in possession</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 78</span></td>
          <td class="col-name"><div class="sec-name">Postponement of prior mortgagee</div></td>
          <td class="col-concept">Prior mortgagee loses priority for fraud/misrepresentation</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Through <strong>fraud, misrepresentation</strong> or <strong>gross neglect</strong> of a prior mortgagee</li>
              <li>Another person induced to advance money on same property</li>
              <li>Prior mortgagee is <strong>postponed</strong> to the subsequent mortgagee</li>
            </ul>
          </td>
          <td class="col-expl expl">If you hold a first mortgage but you fraudulently conceal it or misrepresent the position to a later lender, you lose your priority — the later lender goes first. A prior right must be exercised fairly, not used as a trap.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B (first mortgagee) falsely tells C that the property is unencumbered, inducing C to lend money on a second mortgage. B is postponed to C — C's mortgage is treated as prior.</div></td>
          <td class="col-read"><div class="read-with">S. 48 — priority of rights<br>S. 79 — mortgage securing uncertain amount</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 79</span></td>
          <td class="col-name"><div class="sec-name">Mortgage to secure uncertain amount when maximum is expressed</div></td>
          <td class="col-concept">Running account mortgage — priority up to maximum</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgage to secure future advances/running account (e.g. bank overdraft)</li>
              <li>Maximum amount expressly stated</li>
              <li>Subsequent mortgagee with <strong>notice</strong> of prior mortgage is postponed to prior mortgagee for all advances not exceeding the maximum — even if prior mortgagee makes those advances after receiving notice of subsequent mortgage</li>
            </ul>
          </td>
          <td class="col-expl expl">A bank overdraft mortgage covers future advances up to the stated maximum. A later mortgagee who knows about the overdraft facility cannot claim priority just because the bank later lent more money — as long as it's within the maximum. The later mortgagee took the risk with their eyes open.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration (from Act)</strong>A mortgages Sultanpur to Bank B for overdraft up to Rs.10,000. A then mortgages Sultanpur to C (who has notice of Bank B's mortgage). Bank B can lend up to Rs.10,000 and maintain priority over C for that entire amount.</div></td>
          <td class="col-read"><div class="read-with">S. 78 — prior mortgagee postponed<br>S. 48 — priority of rights</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 80</span></td>
          <td class="col-name"><div class="sec-name">[Tacking abolished] — Repealed</div></td>
          <td class="col-concept">Repealed section</td>
          <td class="col-ingr"><span class="repealed">Repealed by the Transfer of Property (Amendment) Act, 1929, S.41. Abolished the doctrine of tacking (whereby a mortgagee could acquire priority by "tacking" a later advance to an earlier mortgage).</span></td>
          <td class="col-expl expl"><span class="repealed">Now see S.93 — prohibition on tacking.</span></td>
          <td class="col-illus"><div class="illus"><span class="repealed">Refer to S.93 for the current law.</span></div></td>
          <td class="col-read"><div class="read-with">S. 93 — prohibition of tacking</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 81</span></td>
          <td class="col-name"><div class="sec-name">Marshalling securities</div></td>
          <td class="col-concept">Subsequent mortgagee can require prior to exhaust other properties first</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Owner mortgages 2+ properties to one person (prior mortgage)</li>
              <li>Then mortgages one of those to another person (subsequent mortgage)</li>
              <li>Subsequent mortgagee is entitled to have prior mortgage-debt satisfied from property NOT mortgaged to him first</li>
              <li>Provided: not prejudicing prior mortgagee's rights; not prejudicing person who for consideration acquired interest in any of the properties</li>
              <li>Unless contrary contract</li>
            </ul>
          </td>
          <td class="col-expl expl">The second mortgagee gets to choose the order of enforcement — they can insist the first mortgagee go after the other properties first, leaving the second mortgagee's security intact. But the first mortgagee cannot be made worse off.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A mortgages Farms X and Y to B (first mortgage). A then mortgages Farm X to C (second mortgage). C can require B to satisfy his debt from Farm Y first before touching Farm X.</div></td>
          <td class="col-read"><div class="read-with">S. 56 — marshalling by subsequent purchaser (compare)<br>S. 82 — contribution to mortgage debt</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 82</span></td>
          <td class="col-name"><div class="sec-name">Contribution to mortgage-debt</div></td>
          <td class="col-concept">Co-owners contribute to mortgage debt proportionately</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Property subject to a mortgage belongs to 2+ persons with distinct ownership rights</li>
              <li>Each person's share contributes to the mortgage debt rateably (proportionate to value at date of mortgage, after deducting other charges)</li>
              <li>Special rule: if one property paid off one debt and both are mortgaged for another — each contributes rateably to the second after deducting the first debt from the paying property's value</li>
              <li>S.81 (marshalling) property is exempt from this section</li>
            </ul>
          </td>
          <td class="col-expl expl">When co-owned property is mortgaged and one co-owner has to discharge it, the others must contribute proportionally. No one co-owner should bear the entire burden of a debt that encumbers all their shares.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A and B jointly own mortgaged land (A's portion worth Rs.6 lakh; B's worth Rs.4 lakh). Mortgage = Rs.5 lakh. A must pay Rs.3 lakh; B must pay Rs.2 lakh (6:4 ratio).</div></td>
          <td class="col-read"><div class="read-with">S. 81 — marshalling<br>S. 56 — marshalling by purchaser</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 83</span></td>
          <td class="col-name"><div class="sec-name">Power to deposit in Court money due on mortgage. Right to money deposited by mortgagor.</div></td>
          <td class="col-concept">Mortgagor can deposit mortgage money in court</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>After principal money is due; before redemption suit is barred</li>
              <li>Mortgagor (or person entitled to sue for redemption) may deposit mortgage money in court to mortgagee's account</li>
              <li>Court serves notice on mortgagee</li>
              <li>Mortgagee files petition stating amount due + willingness to accept in full discharge + deposits mortgage deed and related documents</li>
              <li>Mortgagee receives money; documents delivered to mortgagor</li>
              <li>If mortgagee in possession: court directs delivery of possession before paying mortgagee</li>
            </ul>
          </td>
          <td class="col-expl expl">If the mortgagee refuses to accept the repayment or cannot be found, the mortgagor can deposit the money in court. This stops interest from running, discharges the mortgage, and protects the mortgagor from being held liable for default when they are ready and willing to pay.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A wants to repay B's mortgage. B refuses to accept payment (hoping to wait for higher interest). A deposits the full amount in the appropriate court. B is notified; interest stops running from the deposit date. A gets the property freed.</div></td>
          <td class="col-read"><div class="read-with">S. 84 — cessation of interest<br>S. 60 — right to redeem</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 84</span></td>
          <td class="col-name"><div class="sec-name">Cessation of interest</div></td>
          <td class="col-concept">Interest stops on tender or deposit</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Interest on principal ceases from: date of <strong>tender</strong>, OR date mortgagor has done all he must do to enable mortgagee to take out the deposited amount (and notice served)</li>
              <li>If deposit made without prior tender and then <strong>withdrawn</strong>: interest runs again from date of withdrawal</li>
              <li>Exception: if mortgagor contracted to give reasonable notice before payment, and notice was not given — mortgagee retains interest entitlement</li>
            </ul>
          </td>
          <td class="col-expl expl">Once the mortgagor properly tenders or deposits the money, the debt stops growing — interest freezes. The mortgagee cannot keep the debt alive by refusing payment or prolonging the process. If the mortgagor withdraws the deposited money, interest resumes from the withdrawal date.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A tenders Rs.5 lakh to B on 1 March. B refuses. A deposits in court on 5 March and completes all formalities. Interest stops on 1 March (date of tender). B cannot claim interest for March and beyond.</div></td>
          <td class="col-read"><div class="read-with">S. 83 — power to deposit<br>S. 60 — right to redeem</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">Ss. 85–90</span></td>
          <td class="col-name"><div class="sec-name">Ss. 85–90 — Parties to suits, Decree in foreclosure, Decree of sale, Procedure, Recovery of balance — All Repealed</div></td>
          <td class="col-concept">Repealed — procedural provisions</td>
          <td class="col-ingr"><span class="repealed">All repealed by the Code of Civil Procedure, 1908 (Act 5 of 1908), S.156 and Schedule V. These sections governed court procedure in foreclosure and redemption suits and have been re-enacted in CPC Order XXXIV.</span></td>
          <td class="col-expl expl"><span class="repealed">Procedure for mortgage suits is now governed by Order XXXIV of the Code of Civil Procedure, 1908 (particularly Rules 1–14). These sections of TPA 1882 are no longer operative.</span></td>
          <td class="col-illus"><div class="illus"><span class="repealed">Refer to CPC Order XXXIV for the current procedural law on mortgage suits.</span></div></td>
          <td class="col-read"><div class="read-with">CPC Order XXXIV — mortgage suits</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 91</span></td>
          <td class="col-name"><div class="sec-name">Persons who may sue for redemption</div></td>
          <td class="col-concept">Who can bring a suit for redemption</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Besides the mortgagor:</li>
              <li><strong>(a)</strong> Any person with any interest in or charge upon the property OR on the right to redeem (except the mortgagee of the interest being redeemed)</li>
              <li><strong>(b)</strong> Any surety for the mortgage debt (or part thereof)</li>
              <li><strong>(c)</strong> Any creditor of the mortgagor who obtained a court decree for sale of the mortgaged property in an administration suit</li>
            </ul>
          </td>
          <td class="col-expl expl">The right to redeem is not exclusive to the mortgagor. Anyone with a stake in the property — a subsequent mortgagee, a guarantor, a creditor — can redeem the mortgage to protect their interest. By redeeming, they get the rights of the mortgagee they paid off (S.92 — subrogation).</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A has mortgaged his property to B. C holds a second mortgage on the same property. If B threatens foreclosure, C can redeem B's mortgage (paying off B) and step into B's position — protecting C's own second mortgage.</div></td>
          <td class="col-read"><div class="read-with">S. 92 — subrogation (right acquired on redemption)<br>S. 60 — mortgagor's right to redeem</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key doctrine">
          <td class="col-sec"><span class="sec-badge">S. 92</span></td>
          <td class="col-name"><div class="sec-name">Subrogation</div><div><span class="tag tag-doctrine">SUBROGATION</span></div></td>
          <td class="col-concept">Doctrine of subrogation — redeemer steps into mortgagee's shoes</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Any of persons in S.91 (other than mortgagor) OR any co-mortgagor redeems</li>
              <li>Acquires the same rights against mortgagor and other mortgagees as the mortgagee who was redeemed</li>
              <li>This right = <strong>right of subrogation</strong></li>
              <li>Also: person who lent money to mortgagor to redeem is subrogated if mortgagor agreed so by <strong>registered instrument</strong></li>
              <li>Subrogation available only if mortgage redeemed <strong>in full</strong></li>
            </ul>
          </td>
          <td class="col-expl expl">Subrogation means "substitution." The person who redeems another's mortgage steps into the mortgagee's position — with all the mortgagee's rights of priority, foreclosure, etc. You don't lose money just because you helped redeem — you gain the same security the mortgagee had.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A's farm is mortgaged: first to B, then to C. C redeems B's first mortgage. C is now subrogated to B's position — C has the first mortgage's priority. A must now deal with C as a first mortgagee and C's original second mortgage as a second mortgage.</div></td>
          <td class="col-read"><div class="read-with">S. 91 — who can redeem<br>S. 93 — prohibition on tacking<br>S. 95 — co-mortgagor's expenses</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 93</span></td>
          <td class="col-name"><div class="sec-name">Prohibition of tacking</div></td>
          <td class="col-concept">No tacking — paying off prior mortgage gives no extra priority</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagee paying off a prior mortgage (with or without notice of intermediate mortgage) acquires NO priority for his original security</li>
              <li>Mortgagee making subsequent advances to mortgagor acquires NO priority for those advances (except as provided by S.79)</li>
            </ul>
          </td>
          <td class="col-expl expl">A mortgagee cannot "tack" (attach) earlier debts to a later priority position to jump ahead of intermediate mortgagees. Each mortgage stands on its own. Paying off a prior mortgage gives you the prior mortgage's position through subrogation (S.92) — not a super-priority.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B (second mortgagee) pays off A's first mortgage to C. B cannot now claim priority of a first mortgagee for B's own original second mortgage debt. B is subrogated to C's first mortgage, but B's own second mortgage remains second.</div></td>
          <td class="col-read"><div class="read-with">S. 92 — subrogation<br>S. 79 — exception (running account)</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 94</span></td>
          <td class="col-name"><div class="sec-name">Rights of mesne mortgagee</div></td>
          <td class="col-concept">Middle mortgagee's rights against subsequent mortgagees</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Property mortgaged for successive debts to successive mortgagees</li>
              <li>Mesne (middle) mortgagee has the same rights against posterior mortgagees as against the mortgagor</li>
            </ul>
          </td>
          <td class="col-expl expl">The middle mortgagee in a chain (e.g. second out of three) is not disadvantaged — they have the same rights against the third mortgagee as they have against the mortgagor. They can require the third mortgagee to redeem them before enforcing.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>Property: first mortgage to B, second to C, third to D. C (mesne mortgagee) has the same rights against D (posterior mortgagee) as against A (mortgagor). D must redeem C before foreclosing.</div></td>
          <td class="col-read"><div class="read-with">S. 91 — persons who may redeem<br>S. 92 — subrogation<br>S. 81 — marshalling</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 95</span></td>
          <td class="col-name"><div class="sec-name">Right of redeeming co-mortgagor to expenses</div></td>
          <td class="col-concept">Co-mortgagor who redeems can recover expenses from others</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>One of several mortgagors redeems the mortgaged property</li>
              <li>In exercising subrogation rights (S.92) against co-mortgagors</li>
              <li>Can add to mortgage money recoverable from co-mortgagors the proportionate redemption expenses attributable to their shares</li>
            </ul>
          </td>
          <td class="col-expl expl">If A and B are co-mortgagors and A pays off the entire mortgage alone, A can recover B's share of the redemption expenses from B — in addition to B's share of the principal. A should not bear B's costs.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A and B co-mortgaged property (50:50). A alone redeems — paying Rs.2 lakh principal + Rs.10,000 legal costs. A can recover Rs.1 lakh + Rs.5,000 from B.</div></td>
          <td class="col-read"><div class="read-with">S. 92 — subrogation<br>S. 82 — contribution to mortgage debt</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 96</span></td>
          <td class="col-name"><div class="sec-name">Mortgage by deposit of title-deeds</div></td>
          <td class="col-concept">Simple mortgage provisions apply to equitable mortgage</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Provisions of simple mortgage (S.58(b)) apply to mortgage by deposit of title-deeds (S.58(f)) as far as may be</li>
            </ul>
          </td>
          <td class="col-expl expl">The equitable mortgage by deposit of title-deeds is governed by the same rules as a simple mortgage, wherever those rules can sensibly apply. This fills the gap left by having no written deed in an equitable mortgage.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A deposits title deeds with bank B (equitable mortgage). Bank B has the same right to sue for a sale of the property on default as a simple mortgagee has — even though there is no written mortgage deed.</div></td>
          <td class="col-read"><div class="read-with">S. 58(b) — simple mortgage<br>S. 58(f) — equitable mortgage<br>S. 59 — registration not required</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 97</span></td>
          <td class="col-name"><div class="sec-name">[Application of proceeds] — Repealed</div></td>
          <td class="col-concept">Repealed — procedural provision</td>
          <td class="col-ingr"><span class="repealed">Repealed by the Code of Civil Procedure, 1908, S.156 and Schedule V. Now re-enacted in CPC Order XXXIV, Rules 12 and 13.</span></td>
          <td class="col-expl expl"><span class="repealed">Application of proceeds from mortgage suits is now governed by CPC Order XXXIV.</span></td>
          <td class="col-illus"><div class="illus"><span class="repealed">Refer to CPC Order XXXIV, Rules 12–13.</span></div></td>
          <td class="col-read"><div class="read-with">CPC Order XXXIV, Rules 12–13</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 98</span></td>
          <td class="col-name"><div class="sec-name">Rights and liabilities of parties to anomalous mortgages</div></td>
          <td class="col-concept">Anomalous mortgage — governed by deed and local usage</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>In case of an anomalous mortgage</li>
              <li>Rights and liabilities determined by: (1) their contract as evidenced in the mortgage deed; (2) so far as contract does not extend: by <strong>local usage</strong></li>
            </ul>
          </td>
          <td class="col-expl expl">Anomalous mortgages don't fit standard categories, so no standard rules can be prescribed. The parties are free to agree on their own terms; what they don't cover, local custom fills. This makes anomalous mortgages highly context-specific.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>An anomalous mortgage in a particular region grants the mortgagee possession plus personal liability. Local usage in that district determines details of possession and recovery that the deed doesn't specify.</div></td>
          <td class="col-read"><div class="read-with">S. 58(g) — anomalous mortgage defined<br>S. 67 — right to foreclose (if deed allows)</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 99</span></td>
          <td class="col-name"><div class="sec-name">[Attachment of mortgaged property] — Repealed</div></td>
          <td class="col-concept">Repealed — procedural provision</td>
          <td class="col-ingr"><span class="repealed">Repealed by the Code of Civil Procedure, 1908, S.156 and Schedule V.</span></td>
          <td class="col-expl expl"><span class="repealed">Governed now by CPC provisions on attachment of property.</span></td>
          <td class="col-illus"><div class="illus"><span class="repealed">Refer to CPC for current law on attachment.</span></div></td>
          <td class="col-read"><div class="read-with">CPC — attachment of property</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="key">
          <td class="col-sec"><span class="sec-badge">S. 100</span></td>
          <td class="col-name"><div class="sec-name">Charges</div></td>
          <td class="col-concept">Charge — security without mortgage</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Immoveable property of one person made security for payment to another</li>
              <li>Transaction does NOT amount to a mortgage</li>
              <li>= <strong>Charge</strong> on the property</li>
              <li>Simple mortgage provisions apply to charges (as far as may be)</li>
              <li>NOT enforceable against transferee for consideration without notice</li>
              <li>Does not apply to trustee's charge on trust property for properly incurred expenses</li>
            </ul>
          </td>
          <td class="col-expl expl">A charge is a lighter form of security — no transfer of interest, but the property is still bound. A court decree for maintenance can create a charge. The main difference from a mortgage is that a charge arises by law or courts, not by transfer of interest by deed. A bona fide buyer without notice takes free from the charge.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A court orders that B's wife is entitled to maintenance from A's property. This creates a charge on A's property in favour of the wife — not a mortgage (A did not "transfer" an interest). A cannot sell to C (who has notice) free of this charge.</div></td>
          <td class="col-read"><div class="read-with">S. 58(a) — mortgage (compare)<br>S. 3 — notice<br>S. 101 — no merger with subsequent encumbrance</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 101</span></td>
          <td class="col-name"><div class="sec-name">No merger in case of subsequent encumbrance</div></td>
          <td class="col-concept">Mortgage/charge does not merge when mortgagee acquires ownership</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Mortgagee (or charge-holder) or their transferee purchases/acquires the rights of the mortgagor/owner</li>
              <li>The mortgage/charge does NOT merge (is not extinguished)</li>
              <li>Protects subsequent mortgagees — they can still enforce their rights</li>
              <li>Subsequent mortgagee/charge-holder cannot foreclose or sell without redeeming the prior mortgage/charge</li>
            </ul>
          </td>
          <td class="col-expl expl">Normally in law, when a lesser right (mortgage) and a greater right (ownership) unite in the same person, the lesser "merges" into the greater and is extinguished. S.101 prevents this in the interest of subsequent mortgagees — the mortgage/charge survives even when the mortgagee acquires ownership, so later creditors are protected.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>B (first mortgagee) buys A's property. B now has both the first mortgage and full ownership. S.101 says B's first mortgage is NOT extinguished — it survives to protect C (second mortgagee), who can still demand that the first mortgage be redeemed before C is shut out.</div></td>
          <td class="col-read"><div class="read-with">S. 100 — charges<br>S. 92 — subrogation</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 102</span></td>
          <td class="col-name"><div class="sec-name">Service or tender on or to agent</div></td>
          <td class="col-concept">Service of notice on agent is sufficient</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>Person to be served does not reside in district where mortgaged property is situated</li>
              <li>Service on agent with general power of attorney (or duly authorised) = sufficient</li>
              <li>If no such person/agent can be found: apply to court for direction on how to serve; service per court's direction = sufficient</li>
              <li>If no person to whom tender should be made can be found: may deposit in court; = tender</li>
            </ul>
          </td>
          <td class="col-expl expl">Practical provision — mortgage parties may be in different districts. Notice to the agent counts. If neither party nor agent can be found, the court guides the process and a court deposit substitutes for a tender.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A wants to tender mortgage money to B, who lives in another state. A can tender to B's agent (who holds a power of attorney) in the district where the property is — equally effective as tendering to B personally.</div></td>
          <td class="col-read"><div class="read-with">S. 83 — deposit in court<br>S. 84 — cessation of interest</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 103</span></td>
          <td class="col-name"><div class="sec-name">Notice, etc., to or by person incompetent to contract</div></td>
          <td class="col-concept">Minors and incapacitated persons — notice/tender handled by curator or court-appointed guardian</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>If notice/tender/deposit involves a person incompetent to contract (minor, lunatic etc.)</li>
              <li>Notice served on/by legal curator of that person's property</li>
              <li>If no curator: apply to court for appointment of guardian ad litem for those purposes</li>
              <li>CPC Order XXXII (guardians for suits) applies as far as may be</li>
            </ul>
          </td>
          <td class="col-expl expl">If one of the mortgage parties is a minor or otherwise legally incapacitated, ordinary notice/tender to/from them is invalid. The law requires going through their legal guardian or a court-appointed guardian for these specific acts.</td>
          <td class="col-illus"><div class="illus"><strong>Illustration</strong>A (minor) is the mortgagor. B wishes to serve notice under S.69. B must serve it on A's legal guardian, not on A directly.</div></td>
          <td class="col-read"><div class="read-with">S. 102 — service on agent<br>CPC Order XXXII — guardians in suits</div></td>
        </tr>

        <tr data-ch="ch4" data-tags="">
          <td class="col-sec"><span class="sec-badge">S. 104</span></td>
          <td class="col-name"><div class="sec-name">Power to make rules</div></td>
          <td class="col-concept">High Court's rule-making power for Chapter IV</td>
          <td class="col-ingr">
            <ul class="ingr-list">
              <li>High Court may from time to time make rules consistent with this Act</li>
              <li>For carrying out Chapter IV provisions in itself and in courts subject to its superintendence</li>
            </ul>
          </td>
          <td class="col-expl expl">Empowers the High Court to make procedural rules for mortgage suits and proceedings within its jurisdiction. Ensures Chapter IV can be practically implemented through locally appropriate court rules.</td>
          <td class="col-illus"><div class="illus"><strong>Note</strong>High Courts across India have issued rules (under their Original Side Rules or Civil Rules of Practice) for filing and conducting mortgage suits under Chapter IV — exercising this S.104 power.</div></td>
          <td class="col-read"><div class="read-with">S. 69A(11) — definition of "the Court" in context of receiver</div></td>
        </tr>

      </tbody>
    </table>
  </div>
</div>

<div class="no-results" id="noResults">No sections match your search or filter.</div>

<footer>
  Transfer of Property Act, 1882 — Act No. 4 of 1882 · Chapters I–IV · Sections 1–104 · All sections covered including repealed sections · Source: Bare Act text.
</footer>

<script>
let currentFilter = 'all';

function toggleChapter(ch) {
  const body = document.getElementById('body-' + ch);
  const tog = document.getElementById('tog-' + ch);
  if (body.style.display === 'none') {
    body.style.display = '';
    tog.textContent = '▼';
  } else {
    body.style.display = 'none';
    tog.textContent = '▶';
  }
}

function setFilter(filter, btn) {
  currentFilter = filter;
  document.querySelectorAll('.filter-btn').forEach(b => b.classList.remove('active'));
  btn.classList.add('active');
  filterTable();
}

function filterTable() {
  const query = document.getElementById('searchInput').value.toLowerCase();
  const rows = document.querySelectorAll('tbody tr');
  let visible = 0;

  rows.forEach(row => {
    const ch = row.dataset.ch || '';
    const tags = (row.dataset.tags || '').split(' ');
    const text = row.textContent.toLowerCase();

    let chMatch = currentFilter === 'all' ||
      currentFilter === ch ||
      (currentFilter === 'key' && tags.includes('key')) ||
      (currentFilter === 'void' && tags.includes('void')) ||
      (currentFilter === 'doctrine' && tags.includes('doctrine'));

    let searchMatch = !query || text.includes(query);

    if (chMatch && searchMatch) {
      row.classList.remove('hidden');
      visible++;
      const grp = document.getElementById('body-' + ch);
      const tog = document.getElementById('tog-' + ch);
      if (grp && grp.style.display === 'none') {
        grp.style.display = '';
        if (tog) tog.textContent = '▼';
      }
    } else {
      row.classList.add('hidden');
    }
  });

  document.getElementById('countLabel').textContent = visible + ' section' + (visible !== 1 ? 's' : '') + ' shown';
  document.getElementById('noResults').style.display = visible === 0 ? 'block' : 'none';
}

window.onload = () => filterTable();
</script>
</body>
</html>
