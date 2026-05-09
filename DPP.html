<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Digital Product Passport — EU ESPR</title>
<link href="https://fonts.googleapis.com/css2?family=DM+Serif+Display:ital@0;1&family=DM+Sans:wght@300;400;500;600&display=swap" rel="stylesheet">
<script src="https://cdnjs.cloudflare.com/ajax/libs/qrcodejs/1.0.0/qrcode.min.js"></script>
<style>
  :root {
    --eu-blue: #003399;
    --eu-gold: #FFCC00;
    --ink: #0d1b2a;
    --mist: #f4f6fb;
    --border: #dde3ef;
  }
  *, *::before, *::after { box-sizing: border-box; margin: 0; padding: 0; }
  body { font-family: 'DM Sans', sans-serif; background: var(--mist); color: var(--ink); min-height: 100vh; }

  /* HEADER */
  header {
    background: linear-gradient(135deg, #001f6b 0%, #003399 60%, #005580 100%);
    color: white; position: relative; overflow: hidden;
  }
  header::before {
    content: ''; position: absolute; inset: 0;
    background: url("data:image/svg+xml,%3Csvg width='60' height='60' viewBox='0 0 60 60' xmlns='http://www.w3.org/2000/svg'%3E%3Cg fill='none'%3E%3Cg fill='%23ffffff' fill-opacity='0.04'%3E%3Ccircle cx='30' cy='30' r='2'/%3E%3C/g%3E%3C/g%3E%3C/svg%3E");
    pointer-events: none;
  }
  .header-inner { max-width: 1100px; margin: 0 auto; padding: 48px 32px 40px; display: flex; align-items: center; gap: 32px; }
  .eu-badge {
    flex-shrink: 0; width: 80px; height: 80px; background: var(--eu-gold);
    border-radius: 50%; display: flex; align-items: center; justify-content: center;
    font-size: 36px; box-shadow: 0 8px 32px rgba(0,0,0,0.3);
    animation: pulse-badge 3s ease-in-out infinite;
  }
  @keyframes pulse-badge { 0%,100%{box-shadow:0 8px 32px rgba(0,0,0,0.3)} 50%{box-shadow:0 12px 48px rgba(255,204,0,0.4)} }
  .header-text h1 { font-family: 'DM Serif Display', serif; font-size: clamp(1.8rem,4vw,2.8rem); line-height: 1.15; letter-spacing: -0.02em; }
  .header-text h1 span { color: var(--eu-gold); font-style: italic; }
  .header-text p { margin-top: 10px; font-size: 0.95rem; opacity: 0.78; font-weight: 300; max-width: 560px; line-height: 1.6; }
  .espr-tag { display: inline-flex; align-items: center; gap: 6px; margin-top: 16px; background: rgba(255,255,255,0.12); border: 1px solid rgba(255,255,255,0.25); padding: 6px 14px; border-radius: 100px; font-size: 0.78rem; font-weight: 500; letter-spacing: 0.05em; text-transform: uppercase; }
  .espr-tag .dot { width: 7px; height: 7px; background: var(--eu-gold); border-radius: 50%; animation: blink 2s infinite; }
  @keyframes blink { 0%,100%{opacity:1} 50%{opacity:0.3} }

  /* STRIP */
  .product-strip { background: white; border-bottom: 2px solid var(--border); }
  .product-strip-inner { max-width: 1100px; margin: 0 auto; padding: 20px 32px; display: flex; align-items: center; justify-content: space-between; flex-wrap: wrap; gap: 16px; }
  .product-info { display: flex; gap: 32px; flex-wrap: wrap; }
  .info-chip { display: flex; flex-direction: column; gap: 2px; }
  .info-chip .label { font-size: 0.72rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.08em; color: #7a87a3; }
  .info-chip .value { font-size: 0.95rem; font-weight: 500; }

  /* TOAST */
  .save-toast {
    position: fixed; bottom: 28px; right: 28px; z-index: 9999;
    background: #1a3a1a; color: white; padding: 12px 20px; border-radius: 12px;
    font-size: 0.85rem; font-weight: 500; display: flex; align-items: center; gap: 8px;
    box-shadow: 0 8px 32px rgba(0,0,0,0.25); opacity: 0; pointer-events: none;
    transform: translateY(12px); transition: all 0.3s ease;
  }
  .save-toast.show { opacity: 1; pointer-events: auto; transform: translateY(0); }

  /* SEARCH */
  .search-bar-wrap { max-width: 1100px; margin: 32px auto 0; padding: 0 32px; }
  .search-bar { display: flex; align-items: center; background: white; border: 1.5px solid var(--border); border-radius: 14px; padding: 0 20px; gap: 12px; box-shadow: 0 2px 12px rgba(0,0,64,0.07); transition: box-shadow 0.2s, border-color 0.2s; }
  .search-bar:focus-within { border-color: var(--eu-blue); box-shadow: 0 4px 24px rgba(0,51,153,0.13); }
  .search-bar input { flex: 1; border: none; outline: none; font-family: 'DM Sans', sans-serif; font-size: 1rem; padding: 16px 0; background: transparent; color: var(--ink); }

  /* GRID */
  .grid-section { max-width: 1100px; margin: 28px auto 0; padding: 0 32px 60px; }
  .section-label { font-size: 0.78rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.1em; color: #7a87a3; margin-bottom: 16px; }
  .category-grid { display: grid; grid-template-columns: repeat(auto-fill, minmax(300px, 1fr)); gap: 16px; }

  /* CARD */
  .cat-card {
    background: white; border: 1.5px solid var(--border); border-radius: 16px; padding: 24px;
    cursor: pointer; transition: transform 0.18s, box-shadow 0.18s, border-color 0.18s;
    position: relative; overflow: hidden; animation: fadeUp 0.4s ease both;
  }
  .cat-card::before { content: ''; position: absolute; top: 0; left: 0; right: 0; height: 3px; background: var(--card-accent, var(--eu-blue)); transform: scaleX(0); transform-origin: left; transition: transform 0.25s ease; }
  .cat-card:hover { transform: translateY(-4px); box-shadow: 0 12px 36px rgba(0,51,153,0.1); border-color: #b8c4e0; }
  .cat-card:hover::before { transform: scaleX(1); }
  @keyframes fadeUp { from{opacity:0;transform:translateY(16px)} to{opacity:1;transform:none} }

  .card-top { display: flex; align-items: flex-start; justify-content: space-between; margin-bottom: 14px; }
  .card-icon { width: 44px; height: 44px; background: var(--icon-bg,#eef1fb); border-radius: 12px; display: flex; align-items: center; justify-content: center; font-size: 1.4rem; }
  .card-num { font-size: 0.7rem; font-weight: 700; color: #aab2c8; letter-spacing: 0.08em; background: var(--mist); padding: 4px 8px; border-radius: 100px; }
  .card-title { font-family: 'DM Serif Display', serif; font-size: 1.05rem; line-height: 1.3; color: var(--ink); margin-bottom: 8px; }
  .card-desc { font-size: 0.83rem; line-height: 1.6; color: #5a6882; font-weight: 300; }
  .card-tags { display: flex; flex-wrap: wrap; gap: 6px; margin-top: 14px; }
  .tag { font-size: 0.7rem; font-weight: 500; padding: 3px 9px; border-radius: 100px; background: var(--icon-bg,#eef1fb); color: var(--card-accent,var(--eu-blue)); letter-spacing: 0.04em; }

  .filled-badge { position: absolute; top: 14px; right: 14px; background: #e6f4ec; color: #2d7a4f; font-size: 0.65rem; font-weight: 700; letter-spacing: 0.06em; padding: 3px 8px; border-radius: 100px; text-transform: uppercase; display: none; }
  .cat-card.has-data .filled-badge { display: block; }

  /* MODAL */
  .modal-overlay { display: none; position: fixed; inset: 0; background: rgba(13,27,42,0.6); backdrop-filter: blur(6px); z-index: 1000; align-items: center; justify-content: center; padding: 24px; }
  .modal-overlay.open { display: flex; }
  .modal { background: white; border-radius: 24px; max-width: 660px; width: 100%; max-height: 88vh; overflow-y: auto; box-shadow: 0 32px 80px rgba(0,0,0,0.25); animation: slideUp 0.3s ease; }
  @keyframes slideUp { from{opacity:0;transform:translateY(32px)} to{opacity:1;transform:none} }

  .modal-header { padding: 28px 28px 20px; border-bottom: 1px solid var(--border); display: flex; align-items: center; gap: 16px; position: sticky; top: 0; background: white; z-index: 10; border-radius: 24px 24px 0 0; }
  .modal-icon { width: 52px; height: 52px; border-radius: 14px; display: flex; align-items: center; justify-content: center; font-size: 1.6rem; flex-shrink: 0; }
  .modal-title { font-family: 'DM Serif Display', serif; font-size: 1.25rem; }
  .modal-subtitle { font-size: 0.72rem; font-weight: 600; text-transform: uppercase; letter-spacing: 0.08em; color: #7a87a3; margin-bottom: 4px; }
  .modal-actions { margin-left: auto; display: flex; gap: 8px; align-items: center; flex-shrink: 0; }

  .btn-save { background: var(--eu-blue); color: white; border: none; border-radius: 10px; padding: 9px 18px; font-family: 'DM Sans', sans-serif; font-size: 0.85rem; font-weight: 600; cursor: pointer; transition: background 0.15s, transform 0.1s; }
  .btn-save:hover { background: #0040bb; }
  .btn-save:active { transform: scale(0.97); }
  .btn-clear { background: #fdecea; color: #b5290a; border: none; border-radius: 10px; padding: 9px 14px; font-family: 'DM Sans', sans-serif; font-size: 0.85rem; font-weight: 600; cursor: pointer; transition: background 0.15s; }
  .btn-clear:hover { background: #fad4d0; }
  .modal-close { width: 34px; height: 34px; border-radius: 50%; border: none; background: var(--mist); cursor: pointer; font-size: 1rem; display: flex; align-items: center; justify-content: center; transition: background 0.15s; }
  .modal-close:hover { background: #dde3ef; }

  .modal-body { padding: 24px 28px 32px; }
  .modal-desc { font-size: 0.88rem; color: #5a6882; line-height: 1.6; margin-bottom: 24px; padding: 14px 16px; background: var(--mist); border-radius: 10px; }

  /* FIELDS */
  .field-group { margin-bottom: 18px; }
  .field-group label { display: block; font-size: 0.72rem; font-weight: 700; text-transform: uppercase; letter-spacing: 0.08em; color: #7a87a3; margin-bottom: 6px; }
  .field-input { width: 100%; border: 1.5px solid var(--border); border-radius: 10px; padding: 11px 14px; font-family: 'DM Sans', sans-serif; font-size: 0.92rem; color: var(--ink); background: white; outline: none; resize: vertical; min-height: 44px; transition: border-color 0.18s, box-shadow 0.18s; line-height: 1.5; }
  .field-input:focus { border-color: var(--eu-blue); box-shadow: 0 0 0 3px rgba(0,51,153,0.08); }
  .field-input.filled { border-color: #b8dfc7; background: #f9fdfa; }
  .field-input::placeholder { color: #b0bace; }

  /* QR */
  .qr-section { background: var(--eu-blue); color: white; padding: 48px 32px; text-align: center; }
  .qr-inner { max-width: 440px; margin: 0 auto; }
  .qr-inner h2 { font-family: 'DM Serif Display', serif; font-size: 1.6rem; margin-bottom: 8px; }
  .qr-inner p { font-size: 0.88rem; opacity: 0.75; margin-bottom: 28px; font-weight: 300; }
  #qrcode { display: inline-block; background: white; padding: 16px; border-radius: 16px; box-shadow: 0 12px 40px rgba(0,0,0,0.3); }
  #qrcode canvas, #qrcode img { display: block; border-radius: 4px; }
  .qr-url { margin-top: 20px; font-size: 0.78rem; opacity: 0.55; font-family: monospace; word-break: break-all; }

  footer { background: var(--ink); color: #8a97b0; padding: 24px 32px; text-align: center; font-size: 0.8rem; line-height: 1.7; }
  footer strong { color: white; }

  @media (max-width: 600px) {
    .header-inner { flex-direction: column; align-items: flex-start; gap: 20px; }
    .category-grid { grid-template-columns: 1fr; }
    .product-info { gap: 16px; }
    .modal-actions { flex-wrap: wrap; }
    .modal-header { flex-wrap: wrap; }
  }
</style>
</head>
<body>

<header>
  <div class="header-inner">
    <div class="eu-badge">♻️</div>
    <div class="header-text">
      <h1>Digital Product <span>Passport</span></h1>
      <p>A comprehensive sustainability and transparency record for textile products, developed in accordance with EU ESPR Regulation 2024/1781.</p>
      <div class="espr-tag"><span class="dot"></span> EU ESPR Compliant · 16 Data Categories</div>
    </div>
  </div>
</header>

<div class="product-strip">
  <div class="product-strip-inner">
    <div class="product-info">
      <div class="info-chip"><span class="label">DPP Version</span><span class="value">v1.0 — 2024</span></div>
      <div class="info-chip"><span class="label">Regulation</span><span class="value">EU ESPR 2024/1781</span></div>
      <div class="info-chip"><span class="label">Sector</span><span class="value">Textile & Apparel</span></div>
      <div class="info-chip"><span class="label">FYP By</span><span class="value">Mudassir · TMM Sem 8</span></div>
    </div>
  </div>
</div>

<div class="search-bar-wrap">
  <div class="search-bar">
    <span style="color:#7a87a3;font-size:1.2rem;">🔍</span>
    <input type="text" id="searchInput" placeholder="Search categories (e.g. sustainability, materials, traceability…)" oninput="filterCards()">
  </div>
</div>

<div class="grid-section">
  <div class="section-label">16 DPP Data Categories — click any card to view &amp; edit</div>
  <div class="category-grid" id="cardGrid"></div>
</div>

<div class="qr-section">
  <div class="qr-inner">
    <h2>Scan to Access This Passport</h2>
    <p>Print or embed this QR code on the product label to give consumers and regulators instant access to the full Digital Product Passport.</p>
    <div id="qrcode"></div>
    <div class="qr-url" id="qrUrl"></div>
  </div>
</div>

<footer>
  <strong>Digital Product Passport — EU ESPR Framework</strong><br>
  Final Year Project · Textile Marketing & Management · 8th Semester<br>
  Based on EU Regulation 2024/1781 (Ecodesign for Sustainable Products Regulation)
</footer>

<!-- MODAL -->
<div class="modal-overlay" id="modalOverlay" onclick="handleOverlayClick(event)">
  <div class="modal">
    <div class="modal-header">
      <div class="modal-icon" id="modalIcon"></div>
      <div>
        <div class="modal-subtitle" id="modalNum"></div>
        <div class="modal-title" id="modalTitle"></div>
      </div>
      <div class="modal-actions">
        <button class="btn-clear" onclick="clearFields()">🗑 Clear</button>
        <button class="btn-save" onclick="saveFields()">💾 Save</button>
        <button class="modal-close" onclick="closeModal()">✕</button>
      </div>
    </div>
    <div class="modal-body" id="modalBody"></div>
  </div>
</div>

<div class="save-toast" id="saveToast"></div>

<script>
const categories = [
  { num:"01", icon:"🏷️", title:"General Product Information", desc:"Core identification data including product name, model, batch/serial number, and manufacturer details.", tags:["Identification","Traceability"], accent:"#003399", iconBg:"#eef1fb",
    fields:[{label:"Product Name / Model",ph:"Enter product name or model number"},{label:"Unique Product Identifier (UUID)",ph:"Auto-generated or manufacturer assigned"},{label:"Batch / Serial Number",ph:"e.g. BATCH-2024-0071"},{label:"Brand / Trade Name",ph:"Enter brand name"},{label:"Date of Manufacture",ph:"YYYY-MM-DD"},{label:"Country of Manufacture",ph:"e.g. Pakistan, Bangladesh, Turkey"}]},
  { num:"02", icon:"🧵", title:"Material Composition", desc:"Detailed breakdown of fibers, substrates, and percentage by weight of all materials used.", tags:["Materials","Fibre Content"], accent:"#2d7a4f", iconBg:"#e6f4ec",
    fields:[{label:"Primary Fiber(s)",ph:"e.g. 100% Cotton / 60% Polyester, 40% Cotton"},{label:"Secondary Components",ph:"e.g. Lining: 100% Viscose"},{label:"Recycled Content (%)",ph:"e.g. 30% recycled polyester"},{label:"Presence of Hazardous Substances",ph:"Yes / No — specify if Yes"},{label:"Certified Standards for Materials",ph:"e.g. GOTS, OEKO-TEX Standard 100"}]},
  { num:"03", icon:"🔬", title:"Chemical Safety & SVHC", desc:"Information on substances of very high concern (SVHC), restricted substances, and REACH compliance.", tags:["REACH","SVHC","Chemicals"], accent:"#b5290a", iconBg:"#fdecea",
    fields:[{label:"SVHC Present (>0.1% w/w)",ph:"Yes / No"},{label:"SVHC List (if applicable)",ph:"CAS numbers and substance names"},{label:"REACH Compliance",ph:"Compliant / Non-compliant — document reference"},{label:"MRSL / RSL Compliance",ph:"e.g. ZDHC MRSL Level 1/2/3"},{label:"Chemical Test Reports",ph:"Link or reference to test certificates"}]},
  { num:"04", icon:"🌱", title:"Environmental Sustainability", desc:"Life cycle assessment data, carbon footprint, water usage, and key environmental impact indicators.", tags:["LCA","Carbon","Water"], accent:"#2d7a4f", iconBg:"#e6f4ec",
    fields:[{label:"Carbon Footprint (kg CO₂e)",ph:"Cradle-to-gate or cradle-to-grave value"},{label:"Water Consumption (litres)",ph:"Total water usage in production"},{label:"Energy Source Used",ph:"Renewable / Non-renewable / Mixed (%)"},{label:"GHG Emissions Category",ph:"Scope 1, 2, 3 — values if available"},{label:"LCA Reference Document",ph:"Link or ISO 14040/14044 report reference"}]},
  { num:"05", icon:"🔁", title:"Circularity & Recyclability", desc:"Design-for-circularity data: recyclability rate, mono-material use, disassembly instructions, end-of-life pathways.", tags:["Circular Economy","End-of-Life"], accent:"#006f8e", iconBg:"#e0f4fa",
    fields:[{label:"Recyclability Rate (%)",ph:"e.g. 85% recyclable by weight"},{label:"Mono-material Construction",ph:"Yes / No"},{label:"Disassembly Instructions",ph:"Describe or provide link"},{label:"End-of-Life Pathway",ph:"Mechanical recycle / Chemical recycle / Compostable / Landfill"},{label:"Take-back Programme Available",ph:"Yes / No — Programme details"}]},
  { num:"06", icon:"🏭", title:"Production & Manufacturing", desc:"Manufacturing site information, production processes, certifications, and key supply chain actors.", tags:["Production","Suppliers"], accent:"#5b3e8e", iconBg:"#f0eafa",
    fields:[{label:"Manufacturer Name",ph:"Legal name of manufacturing entity"},{label:"Facility Address & Country",ph:"Full address of production facility"},{label:"Production Process Description",ph:"e.g. Ring spun, Reactive dyeing, Pre-washing"},{label:"Manufacturing Certifications",ph:"e.g. ISO 9001, SA8000, WRAP"},{label:"Subcontractors Used",ph:"List names/locations if applicable"}]},
  { num:"07", icon:"🔍", title:"Traceability & Supply Chain", desc:"Full supply chain mapping from raw material origin to finished product, with tier-by-tier transparency.", tags:["Supply Chain","Transparency"], accent:"#003399", iconBg:"#eef1fb",
    fields:[{label:"Tier 1 — Assembly / Cut & Sew",ph:"Facility name, country"},{label:"Tier 2 — Fabric / Yarn Production",ph:"Facility name, country"},{label:"Tier 3 — Raw Material Origin",ph:"Farm / Fibre source, country"},{label:"Supply Chain Verification Method",ph:"Third-party audit / Blockchain / Self-declaration"},{label:"Chain of Custody Certificate",ph:"Certificate number or link"}]},
  { num:"08", icon:"🏅", title:"Certifications & Standards", desc:"All third-party certifications, eco-labels, social standards, and quality marks applicable to the product.", tags:["Labels","Standards","Certifications"], accent:"#c47d0a", iconBg:"#fef8e8",
    fields:[{label:"Environmental Certifications",ph:"e.g. GOTS, bluesign®, Cradle to Cradle"},{label:"Social Certifications",ph:"e.g. Fair Trade, SA8000, Better Cotton"},{label:"Quality Certifications",ph:"e.g. OEKO-TEX STANDARD 100, ISO"},{label:"Certification Bodies",ph:"Names of certifying organisations"},{label:"Certificate Validity Period",ph:"Valid from — Valid until"},{label:"Certificate Documents / Links",ph:"Uploaded or URL references"}]},
  { num:"09", icon:"⚙️", title:"Durability & Repairability", desc:"Expected product lifespan, durability test results, availability of spare parts, and repair guidance.", tags:["Durability","Repair"], accent:"#7a5c00", iconBg:"#faf3e0",
    fields:[{label:"Expected Lifespan (years)",ph:"Design or tested lifespan"},{label:"Durability Test Results",ph:"Pilling, Tear strength, Colour fastness grades"},{label:"Care & Maintenance Instructions",ph:"Washing, drying, ironing guidance"},{label:"Repairability Score",ph:"Score or rating if applicable"},{label:"Spare Parts / Repair Services Available",ph:"Yes / No — details"}]},
  { num:"10", icon:"🚚", title:"Packaging & Logistics", desc:"Packaging materials, sustainability of packaging, transport emissions, and logistics chain data.", tags:["Packaging","Transport"], accent:"#006f8e", iconBg:"#e0f4fa",
    fields:[{label:"Packaging Material",ph:"e.g. Recycled cardboard, biodegradable polybag"},{label:"Packaging Recyclability",ph:"Yes / No / Partially"},{label:"Packaging Weight (g)",ph:"Primary + Secondary packaging weight"},{label:"Transport Mode",ph:"Sea / Air / Road / Rail"},{label:"Logistics Carbon Footprint",ph:"kg CO₂e per unit if available"}]},
  { num:"11", icon:"👷", title:"Social & Labour Compliance", desc:"Labour rights, working conditions, wages, freedom of association, and responsible sourcing practices.", tags:["Labour Rights","Social"], accent:"#b5290a", iconBg:"#fdecea",
    fields:[{label:"Living Wage Commitment",ph:"Yes / No / In Progress"},{label:"Working Hours Compliance",ph:"Max hours/week — ILO compliant?"},{label:"Freedom of Association",ph:"Policy in place: Yes / No"},{label:"Child Labour Policy",ph:"Zero tolerance — verification method"},{label:"Gender Equality Initiatives",ph:"Describe programmes if applicable"},{label:"Social Audit Conducted By",ph:"Auditor name, date"}]},
  { num:"12", icon:"🎨", title:"Product Care & Use Instructions", desc:"Consumer-facing care labels, proper use information, and guidance to extend product life.", tags:["Care Label","Consumer Info"], accent:"#5b3e8e", iconBg:"#f0eafa",
    fields:[{label:"Washing Instructions",ph:"e.g. 30°C machine wash, gentle cycle"},{label:"Drying Instructions",ph:"e.g. Tumble dry low / Line dry"},{label:"Ironing",ph:"e.g. Medium heat / Do not iron"},{label:"Dry Cleaning",ph:"Allowed / Not recommended"},{label:"Storage Recommendations",ph:"e.g. Cool dry place, hang or fold"},{label:"Care Symbol Reference",ph:"ISO 3758 symbols used"}]},
  { num:"13", icon:"📋", title:"Regulatory Compliance", desc:"Compliance declarations with EU and international regulations applicable to textile and apparel products.", tags:["Compliance","Legal"], accent:"#003399", iconBg:"#eef1fb",
    fields:[{label:"EU Textile Labelling Regulation",ph:"Regulation (EU) No 1007/2011 — Compliant?"},{label:"ESPR Compliance Status",ph:"Full / Partial / In Progress"},{label:"CE Marking (if applicable)",ph:"Yes / No"},{label:"REACH Compliance Declaration",ph:"Document reference or link"},{label:"Country-specific Regulations Met",ph:"List applicable national regulations"},{label:"Responsible Person in EU",ph:"Name and contact of EU representative"}]},
  { num:"14", icon:"🗑️", title:"End-of-Life & Waste Management", desc:"Instructions for disposal, recycling channels, composting eligibility, and waste diversion options.", tags:["End-of-Life","Waste"], accent:"#2d7a4f", iconBg:"#e6f4ec",
    fields:[{label:"Recommended Disposal Method",ph:"Textile bank / Kerbside recycle / Compost"},{label:"Nearest Textile Recycling Point",ph:"Locator URL or description"},{label:"Compostable / Biodegradable",ph:"Yes / No — conditions required"},{label:"Take-back / Refund Scheme",ph:"Details of manufacturer take-back"},{label:"Hazardous Waste Considerations",ph:"Any special disposal requirements?"}]},
  { num:"15", icon:"📊", title:"Digital & Data Governance", desc:"Data ownership, access rights, DPP update log, data formats, and system interoperability details.", tags:["Data","Governance"], accent:"#c47d0a", iconBg:"#fef8e8",
    fields:[{label:"DPP Issued By",ph:"Organisation / System name"},{label:"Data Standard Used",ph:"e.g. GS1, CIRPASS, W3C DID"},{label:"Last Updated",ph:"YYYY-MM-DD"},{label:"Access Level",ph:"Public / Restricted / Regulator only"},{label:"Interoperability Format",ph:"JSON-LD / XML / API endpoint"},{label:"Data Retention Period",ph:"e.g. 10 years post end-of-life"}]},
  { num:"16", icon:"📢", title:"Consumer Transparency & Claims", desc:"Verified sustainability claims, greenwashing safeguards, and consumer-facing communication data.", tags:["Claims","Transparency"], accent:"#006f8e", iconBg:"#e0f4fa",
    fields:[{label:"Sustainability Claims Made",ph:"List all public-facing claims"},{label:"Verification of Claims",ph:"How each claim is substantiated"},{label:"Third-party Verification Body",ph:"Name of verifier or auditor"},{label:"EU Green Claims Directive Alignment",ph:"Aligned / Not yet / In review"},{label:"QR / DPP Link on Label",ph:"Yes / No — label placement"},{label:"Consumer Helpdesk / Contact",ph:"Email, phone, or web URL"}]},
];

const STORAGE_KEY = 'dpp_data_v1';
function loadData() { try { return JSON.parse(localStorage.getItem(STORAGE_KEY)) || {}; } catch { return {}; } }
function persistData(d) { localStorage.setItem(STORAGE_KEY, JSON.stringify(d)); }
function cardHasData(num) { const d = loadData()[`cat_${num}`]; return d && Object.values(d).some(v => v && v.trim()); }

function renderCards(list) {
  const grid = document.getElementById('cardGrid');
  grid.innerHTML = '';
  list.forEach((cat, i) => {
    const div = document.createElement('div');
    div.className = 'cat-card' + (cardHasData(cat.num) ? ' has-data' : '');
    div.style.setProperty('--card-accent', cat.accent);
    div.style.setProperty('--icon-bg', cat.iconBg);
    div.style.animationDelay = (i * 0.04) + 's';
    div.innerHTML = `
      <span class="filled-badge">✔ Filled</span>
      <div class="card-top">
        <div class="card-icon">${cat.icon}</div>
        <div class="card-num">CAT ${cat.num}</div>
      </div>
      <div class="card-title">${cat.title}</div>
      <div class="card-desc">${cat.desc}</div>
      <div class="card-tags">${cat.tags.map(t=>`<span class="tag">${t}</span>`).join('')}</div>
    `;
    div.addEventListener('click', () => openModal(cat));
    grid.appendChild(div);
  });
  if (!list.length) grid.innerHTML = '<div style="grid-column:1/-1;text-align:center;padding:48px;color:#7a87a3;">No categories match your search.</div>';
}

function filterCards() {
  const q = document.getElementById('searchInput').value.toLowerCase();
  renderCards(q ? categories.filter(c => c.title.toLowerCase().includes(q) || c.desc.toLowerCase().includes(q) || c.tags.some(t=>t.toLowerCase().includes(q))) : categories);
}

let currentCat = null;

function openModal(cat) {
  currentCat = cat;
  const saved = loadData()[`cat_${cat.num}`] || {};
  document.getElementById('modalIcon').textContent = cat.icon;
  document.getElementById('modalIcon').style.background = cat.iconBg;
  document.getElementById('modalNum').textContent = `Category ${cat.num} · ${cat.tags.join(' · ')}`;
  document.getElementById('modalTitle').textContent = cat.title;
  document.getElementById('modalBody').innerHTML = `<div class="modal-desc">${cat.desc}</div>` +
    cat.fields.map((f,idx) => {
      const val = saved[`f${idx}`] || '';
      return `<div class="field-group">
        <label>${f.label}</label>
        <textarea class="field-input ${val?'filled':''}" rows="2" placeholder="${f.ph}" data-idx="${idx}"
          oninput="this.classList.toggle('filled',this.value.trim()!=='')">${val}</textarea>
      </div>`;
    }).join('');
  document.getElementById('modalOverlay').classList.add('open');
}

function saveFields() {
  if (!currentCat) return;
  const d = loadData();
  const key = `cat_${currentCat.num}`;
  d[key] = {};
  document.querySelectorAll('.field-input').forEach(el => { d[key][`f${el.dataset.idx}`] = el.value; });
  persistData(d);
  showToast('✅ Saved successfully!');
  renderCards(categories);
}

function clearFields() {
  if (!currentCat || !confirm('Clear all fields in this category?')) return;
  const d = loadData();
  delete d[`cat_${currentCat.num}`];
  persistData(d);
  document.querySelectorAll('.field-input').forEach(el => { el.value=''; el.classList.remove('filled'); });
  renderCards(categories);
  showToast('🗑 Fields cleared.');
}

function closeModal() { document.getElementById('modalOverlay').classList.remove('open'); }
function handleOverlayClick(e) { if (e.target===document.getElementById('modalOverlay')) closeModal(); }
document.addEventListener('keydown', e => { if (e.key==='Escape') closeModal(); });

function showToast(msg) {
  const t = document.getElementById('saveToast');
  t.textContent = msg; t.classList.add('show');
  setTimeout(() => t.classList.remove('show'), 2500);
}

renderCards(categories);

const pageUrl = window.location.href;
document.getElementById('qrUrl').textContent = pageUrl;
new QRCode(document.getElementById('qrcode'), { text: pageUrl, width: 220, height: 220, colorDark:"#003399", colorLight:"#ffffff", correctLevel: QRCode.CorrectLevel.M });
</script>
</body>
</html>
