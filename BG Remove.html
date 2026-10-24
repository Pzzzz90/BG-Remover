<!doctype html>
<html lang="th">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width,initial-scale=1,viewport-fit=cover">
<meta name="theme-color" content="#0f1115">
<title>ลบพื้นหลังภาพ</title>
<style>
:root{--bg:#0f1115;--panel:#181b22;--line:#2a2f3a;--tx:#e8eaf0;--mut:#9aa3b2;--ac:#4f8cff;--ok:#2ecc71;--er:#ff5d5d;--wn:#f5a623}
*{box-sizing:border-box;-webkit-tap-highlight-color:transparent}
body{margin:0;background:var(--bg);color:var(--tx);font:15px/1.5 system-ui,"Noto Sans Thai",sans-serif}
.wrap{max-width:1100px;margin:0 auto;padding:12px 12px calc(28px + env(safe-area-inset-bottom))}
h1{font-size:18px;margin:4px 0 10px;display:flex;align-items:center;gap:8px;flex-wrap:wrap}
.chip{font-size:12px;font-weight:400;color:var(--mut);border:1px solid var(--line);border-radius:99px;padding:2px 10px}
button,select,input{font:inherit;color:inherit}
.btn{min-height:44px;padding:0 14px;border-radius:10px;border:1px solid var(--line);background:var(--panel);cursor:pointer;white-space:nowrap}
.btn.pri{background:var(--ac);border-color:var(--ac);color:#fff;font-weight:600}
.btn.dng{border-color:var(--er);color:var(--er)}
.btn[disabled]{opacity:.4;cursor:not-allowed}
.btn.on{outline:2px solid var(--ac);background:#1c2a47}
.row{display:flex;flex-wrap:wrap;gap:8px;align-items:center;margin:8px 0}
.row.grow>*{flex:1 1 auto}
.card{background:var(--panel);border:1px solid var(--line);border-radius:12px;padding:10px 12px;margin:10px 0}
.card h2{font-size:14px;margin:0 0 6px;color:var(--mut);font-weight:600}
#drop{border:2px dashed var(--line);border-radius:12px;padding:14px;text-align:center;color:var(--mut)}
#drop.over{border-color:var(--ac);background:#14213b}
#msg{display:none;border-radius:10px;padding:10px 12px;margin:8px 0;border:1px solid;align-items:flex-start;gap:10px}
#msg.show{display:flex}
#msg.err{border-color:var(--er);background:#2a1414}
#msg.warn{border-color:var(--wn);background:#2a2010}
#msg.info{border-color:var(--ac);background:#10203a}
#msg span{flex:1;white-space:pre-line}
#msg button{background:none;border:0;color:var(--mut);font-size:18px;cursor:pointer;min-width:32px;min-height:32px}
#prog{display:none;margin:8px 0}
#prog.show{display:block}
#bar{height:8px;background:#232834;border-radius:99px;overflow:hidden}
#bar i{display:block;height:100%;width:0;background:var(--ac);transition:width .2s}
#bar.ind i{width:40%;animation:ind 1.1s infinite ease-in-out}
@keyframes ind{0%{margin-left:-40%}100%{margin-left:100%}}
#progtxt{font-size:13px;color:var(--mut);margin-top:4px}
#viewport{position:relative;height:min(62vh,640px);min-height:320px;background:#0a0b0e;border:1px solid var(--line);border-radius:12px;overflow:hidden;touch-action:none;user-select:none;-webkit-user-select:none}
#empty{position:absolute;inset:0;display:flex;align-items:center;justify-content:center;color:var(--mut);text-align:center;padding:20px;pointer-events:none}
#stage{position:absolute;left:0;top:0;transform-origin:0 0;will-change:transform;display:none}
#stage.px canvas{image-rendering:pixelated}
#stage canvas{position:absolute;left:0;top:0;display:block}
#resWrap{position:absolute;left:0;top:0;--ck:16px;background-color:#fff;
 background-image:linear-gradient(45deg,#c4c8d0 25%,transparent 25%,transparent 75%,#c4c8d0 75%),linear-gradient(45deg,#c4c8d0 25%,transparent 25%,transparent 75%,#c4c8d0 75%);
 background-size:calc(var(--ck)*2) calc(var(--ck)*2);background-position:0 0,var(--ck) var(--ck)}
#resWrap.bg-white{background-image:none;background-color:#fff}
#resWrap.bg-black{background-image:none;background-color:#000}
#resWrap.bg-green{background-image:none;background-color:#12b04a}
#divider{position:absolute;top:0;bottom:0;width:calc(2px / var(--s,1));background:#fff;box-shadow:0 0 0 calc(1px / var(--s,1)) #000;display:none;pointer-events:none}
#cursor{position:absolute;border:2px solid #fff;border-radius:50%;box-shadow:0 0 0 1px #000;pointer-events:none;display:none;transform:translate(-50%,-50%)}
#zoomlbl{position:absolute;right:8px;bottom:8px;background:#000a;border-radius:6px;padding:2px 8px;font-size:12px;pointer-events:none}
.seg{display:flex;flex-wrap:wrap;gap:6px}
.seg .btn{flex:1 1 auto;padding:0 10px}
label.f{display:flex;align-items:center;gap:8px;flex:1 1 200px;font-size:13px;color:var(--mut)}
label.f input[type=range]{flex:1;min-height:32px}
select{min-height:44px;border-radius:10px;border:1px solid var(--line);background:var(--panel);padding:0 8px}
#cmpRow{display:none}
details summary{cursor:pointer;color:var(--mut);min-height:32px}
details p,details li{font-size:13px;color:var(--mut);margin:4px 0}
.kv{font-size:13px;color:var(--mut)}
.chk{display:flex;align-items:center;gap:8px;min-height:36px;font-size:14px}
.chk input{width:20px;height:20px}
</style>
</head>
<body>
<div class="wrap">
 <h1>ลบพื้นหลังภาพ <span class="chip" id="chipBackend">ยังไม่โหลดโมเดล</span> <span class="chip">ภาพไม่ถูกอัปโหลดไปไหน</span></h1>

 <div id="msg" role="alert"><span id="msgtxt"></span><button id="msgx" aria-label="ปิด">×</button></div>

 <div class="card">
  <div id="drop">
   <div class="row" style="justify-content:center">
    <button class="btn pri" id="pick">เลือกรูปจากอุปกรณ์</button>
    <button class="btn" id="pasteBtn">วางจากคลิปบอร์ด</button>
   </div>
   <div style="font-size:13px">หรือลากรูปมาวางที่นี่ · วาง (Ctrl+V) · รองรับ JPG / PNG / WebP</div>
   <input type="file" id="file" accept="image/jpeg,image/png,image/webp" hidden>
  </div>
  <div class="kv" id="imgInfo" style="margin-top:6px"></div>
 </div>

 <div class="row grow">
  <button class="btn pri" id="run" disabled>ลบพื้นหลัง</button>
  <button class="btn dng" id="cancel" disabled>ยกเลิก</button>
 </div>
 <div id="prog"><div id="bar"><i></i></div><div id="progtxt"></div></div>

 <div class="card">
  <h2>มุมมอง</h2>
  <div class="seg" id="modes">
   <button class="btn on" data-mode="result">ผลลัพธ์</button>
   <button class="btn" data-mode="orig">ต้นฉบับ</button>
   <button class="btn" data-mode="compare">เปรียบเทียบ</button>
   <button class="btn" data-mode="mask">หน้ากาก</button>
   <button class="btn" data-mode="overlay">พื้นที่ที่ลบ</button>
  </div>
  <div class="row" id="cmpRow"><label class="f">ก่อน ◀ <input type="range" id="cmp" min="0" max="100" value="50"> ▶ หลัง</label></div>
  <div class="row">
   <label class="f" style="flex:0 0 auto">พื้นหลังแสดงผล
    <select id="bg"><option value="">ตารางหมากรุก</option><option value="bg-white">ขาว</option><option value="bg-black">ดำ</option><option value="bg-green">เขียว</option></select>
   </label>
  </div>
 </div>

 <div id="viewport">
  <div id="empty">ยังไม่มีรูป — เลือกรูปเพื่อเริ่มต้น</div>
  <div id="stage">
   <canvas id="cOrig"></canvas>
   <div id="resWrap"><canvas id="cRes"></canvas></div>
   <div id="divider"></div>
  </div>
  <div id="cursor"></div>
  <div id="zoomlbl">100%</div>
 </div>

 <div class="row grow">
  <button class="btn" id="zin" disabled>＋ ซูมเข้า</button>
  <button class="btn" id="zout" disabled>－ ซูมออก</button>
  <button class="btn" id="zfit" disabled>Fit to Screen</button>
  <button class="btn" id="zreset" disabled>Reset Zoom</button>
 </div>

 <div class="card">
  <h2>แก้ไขหน้ากาก (แก้เฉพาะ Alpha ไม่แตะสี RGB)</h2>
  <div class="seg" id="tools">
   <button class="btn on" data-tool="pan">✋ เลื่อนดู</button>
   <button class="btn" data-tool="restore" disabled>🖌 Brush คืนวัตถุ</button>
   <button class="btn" data-tool="erase" disabled>🧽 Eraser ลบพื้นหลัง</button>
  </div>
  <div class="row">
   <label class="f">ขนาดแปรง <input type="range" id="bsize" min="6" max="160" value="40"><b id="bsizeV">40</b></label>
   <label class="f">ความนุ่ม <input type="range" id="bsoft" min="0" max="100" value="30"><b id="bsoftV">30</b></label>
  </div>
  <div class="seg">
   <button class="btn" id="undo" disabled>↶ Undo</button>
   <button class="btn" id="redo" disabled>↷ Redo</button>
   <button class="btn dng" id="resetMask" disabled>Reset Mask</button>
  </div>
  <div class="kv" style="margin-top:6px">นิ้วเดียว = วาด/เลื่อน (ตามเครื่องมือ) · สองนิ้ว = ซูมและเลื่อนเสมอ</div>
 </div>

 <div class="card">
  <h2>โมเดลและการส่งออก</h2>
  <div class="row">
   <label class="f" style="flex:0 0 auto">โหมดโมเดล
    <select id="quality">
     <option value="auto">อัตโนมัติ (GPU แม่นยำ / CPU ประหยัด)</option>
     <option value="fp32">แม่นยำสุด (≈176 MB, ช้ากว่าบน CPU)</option>
     <option value="q8">ประหยัด (≈44 MB, CPU เท่านั้น)</option>
    </select>
   </label>
  </div>
  <label class="chk"><input type="checkbox" id="decon"> กำจัดสีพื้นหลังที่ติดขอบ (ปรับเฉพาะพิกเซลขอบกึ่งโปร่งใสตอนส่งออก)</label>
  <div class="row grow">
   <button class="btn pri" id="dl" disabled>ดาวน์โหลด PNG โปร่งใส</button>
  </div>
  <div class="kv" id="expInfo"></div>
 </div>

 <details class="card">
  <summary>ข้อมูลการทำงาน ความเป็นส่วนตัว และข้อจำกัด</summary>
  <ul>
   <li>ภาพของคุณประมวลผลในเครื่องทั้งหมด ไม่ถูกส่งไปเซิร์ฟเวอร์ใด ๆ ที่ดาวน์โหลดมีเฉพาะไลบรารี (jsDelivr) และไฟล์โมเดล (Hugging Face)</li>
   <li>ต้องใช้อินเทอร์เน็ตครั้งแรกเพื่อโหลดไลบรารีและโมเดล (≈44–176 MB) หลังจากนั้นเบราว์เซอร์จะแคชโมเดลไว้ จึงลบพื้นหลังแบบออฟไลน์ได้หากแคชยังอยู่และเปิดผ่าน HTTPS/localhost</li>
   <li>ดู/ซูม/แก้หน้ากาก/ส่งออก PNG ทำงานออฟไลน์ได้เสมอเมื่อโหลดรูปแล้ว</li>
   <li>เปิดผ่าน file:// แคชโมเดลอาจใช้ไม่ได้และ WebGPU ไม่ทำงาน ควรเปิดผ่าน localhost หรือ HTTPS</li>
   <li>โมเดล briaai/RMBG-1.4 ใช้ได้ไม่เชิงพาณิชย์ (CC BY-NC 4.0) หากใช้งานธุรกิจต้องตรวจสอบ/ซื้อสิทธิ์ หรือเปลี่ยนค่า CFG.MODEL เป็นโมเดลที่ใบอนุญาตเหมาะสม</li>
   <li>ส่งออกเป็นไฟล์ PNG ที่เข้ารหัสเอง: RGB ต้นฉบับถูกเก็บตามเดิมทุกพิกเซล เปลี่ยนเฉพาะ Alpha (ยกเว้นเปิดตัวเลือกกำจัดสีขอบ) ขนาดภาพเท่าต้นฉบับ</li>
   <li>ภาพใหญ่เกิน 12 ล้านพิกเซลอาจช้าหรือหน่วยความจำไม่พอบนมือถือ ระบบรองรับสูงสุด ≈36 ล้านพิกเซล</li>
  </ul>
 </details>
</div>

<script type="text/plain" id="workerSrc">
let lib=null,model=null,Tensor=null,backend='',cfg=null;
const post=(m,t)=>self.postMessage(m,t||[]);
const tag=(e,code)=>{const x=e instanceof Error?e:new Error(String(e));if(!x.code)x.code=code;return x};
async function load(attempts){
  const files={};
  const cb=p=>{
    if(p.status==='progress'&&p.total){
      files[p.file]={l:p.loaded,t:p.total};
      let L=0,T=0;for(const k in files){L+=files[k].l;T+=files[k].t}
      post({type:'progress',pct:T?L/T*100:null,text:'กำลังดาวน์โหลดโมเดล '+(L/1048576).toFixed(0)+' / '+(T/1048576).toFixed(0)+' MB'});
    }else if(p.status==='ready'){post({type:'progress',pct:null,text:'กำลังเตรียมโมเดล…'})}
  };
  let last;
  for(const a of attempts){
    try{
      post({type:'progress',pct:null,text:'กำลังโหลดโมเดล ('+(a.device==='webgpu'?'GPU':'CPU')+')…'});
      model=await lib.AutoModel.from_pretrained(cfg.model,{config:{model_type:'custom'},device:a.device,dtype:a.dtype,progress_callback:cb});
      backend=a.device+' / '+a.dtype;
      return;
    }catch(e){last=e;model=null}
  }
  throw tag(last,'MODEL');
}
async function init(m){
  cfg=m;
  if(!lib){
    post({type:'progress',pct:null,text:'กำลังโหลดไลบรารี AI…'});
    try{lib=await import(m.lib)}catch(e){throw tag(e,'LIB')}
    lib.env.allowLocalModels=false;lib.env.useBrowserCache=true;Tensor=lib.Tensor;
  }
  if(!model){
    const att=[];
    if(m.hasGPU&&m.quality!=='q8')att.push({device:'webgpu',dtype:'fp32'});
    att.push({device:'wasm',dtype:m.quality==='fp32'?'fp32':'q8'});
    await load(att);
  }
  post({type:'ready',backend});
}
async function infer(t){
  const out=await model({input:t});
  const o=out.output||out[Object.keys(out)[0]];
  const d=o.data;
  const N=1024*1024;
  if(!d||d.length!==N)throw tag(new Error('unexpected output size '+(d&&d.length)),'INFER');
  const mask=new Uint8ClampedArray(N);
  for(let i=0;i<N;i++){const v=d[i];mask[i]=v<0?0:v>1?255:v*255}
  for(const k in out){try{out[k].dispose&&out[k].dispose()}catch(_){}}
  return mask;
}
async function run(m){
  const px=new Uint8ClampedArray(m.buf),N=1024*1024,f=new Float32Array(3*N);
  for(let i=0;i<N;i++){const j=i*4;f[i]=px[j]/255-.5;f[N+i]=px[j+1]/255-.5;f[2*N+i]=px[j+2]/255-.5}
  const t=new Tensor('float32',f,[1,3,1024,1024]);
  let mask;
  try{mask=await infer(t)}
  catch(e){
    if(backend.indexOf('webgpu')===0){
      post({type:'progress',pct:null,text:'GPU ใช้ไม่ได้ กำลังสลับไปใช้ CPU…'});
      model=null;await load([{device:'wasm',dtype:cfg.quality==='fp32'?'fp32':'q8'}]);
      post({type:'backend',backend});
      mask=await infer(t);
    }else throw e;
  }
  try{t.dispose&&t.dispose()}catch(_){}
  post({type:'done',id:m.id,buf:mask.buffer},[mask.buffer]);
}
self.onmessage=async e=>{
  const m=e.data;
  try{if(m.type==='init')await init(m);else if(m.type==='run')await run(m)}
  catch(err){
    const msg=String(err&&err.message||err);
    const code=err&&err.code||(/memory|alloc|OOM/i.test(msg)?'OOM':'INFER');
    post({type:'error',id:m.id,code,message:msg});
  }
};
</script>

<script>
'use strict';
const CFG={LIB:'https://cdn.jsdelivr.net/npm/@huggingface/transformers@3.0.2',MODEL:'briaai/RMBG-1.4',MAX_PX:36e6,WARN_PX:12e6,TILE:64,HIST:40};
const $=s=>document.querySelector(s);
class AppError extends Error{constructor(code,msg){super(msg);this.code=code}}

const S={name:'image',W:0,H:0,orig:null,origA:null,mask:null,base:null,hist:[],redo:[],
  mode:'result',tool:'pan',v:{s:1,x:0,y:0},fitS:1,cmp:50,busy:false,exporting:false,
  ready:false,worker:null,pending:{},initP:null,backend:''};

const vp=$('#viewport'),stage=$('#stage'),cOrig=$('#cOrig'),cRes=$('#cRes'),resWrap=$('#resWrap'),divider=$('#divider'),cursor=$('#cursor');
const ctxRes=cRes.getContext('2d');

/* ---------- UI helpers ---------- */
function msg(type,text){const m=$('#msg');m.className='show '+type;$('#msgtxt').textContent=text;m.classList.add('show')}
function clearMsg(){$('#msg').className=''}
$('#msgx').onclick=clearMsg;
function setProgress(pct,text){
  $('#prog').classList.add('show');
  const bar=$('#bar');
  if(pct==null){bar.classList.add('ind')}else{bar.classList.remove('ind');bar.firstElementChild.style.width=Math.max(2,Math.min(100,pct))+'%'}
  $('#progtxt').textContent=text||'';
}
function hideProgress(){$('#prog').classList.remove('show')}
function fmtBytes(n){return n>=1048576?(n/1048576).toFixed(2)+' MB':(n/1024).toFixed(0)+' KB'}
function updateUI(){
  const has=!!S.orig,hasMask=!!S.mask;
  $('#run').disabled=!has||S.busy;
  $('#cancel').disabled=!S.busy;
  $('#pick').disabled=S.busy;
  for(const id of ['zin','zout','zfit','zreset'])$('#'+id).disabled=!has;
  for(const b of document.querySelectorAll('#tools [data-tool="restore"],#tools [data-tool="erase"]'))b.disabled=!hasMask||S.busy;
  $('#undo').disabled=!S.hist.length||S.busy;
  $('#redo').disabled=!S.redo.length||S.busy;
  $('#resetMask').disabled=!hasMask||S.busy;
  $('#dl').disabled=!hasMask||S.busy||S.exporting;
  $('#run').textContent=S.busy?'กำลังประมวลผล…':(hasMask?'ลบพื้นหลังใหม่อีกครั้ง':'ลบพื้นหลัง');
}
function humanError(e){
  const code=e&&e.code;
  if(code==='ABORT')return 'ยกเลิกการประมวลผลแล้ว';
  if(code==='LIB')return (navigator.onLine?'โหลดไลบรารี AI ไม่สำเร็จ':'ไม่มีอินเทอร์เน็ต และยังไม่มีไลบรารีในแคช')+'\nวิธีแก้: เชื่อมต่ออินเทอร์เน็ต แล้วเปิดหน้านี้ผ่าน localhost หรือ HTTPS (ไม่ใช่ file://) จากนั้นกดลองใหม่';
  if(code==='MODEL')return (navigator.onLine?'โหลดโมเดลไม่สำเร็จ':'ออฟไลน์ และโมเดลยังไม่ถูกแคชไว้')+'\nวิธีแก้: เชื่อมต่อ Wi-Fi ที่เสถียร ตรวจพื้นที่ว่างในเครื่อง หรือเลือกโหมดโมเดล "ประหยัด" แล้วลองใหม่';
  if(code==='WORKER')return 'เบราว์เซอร์นี้เริ่มตัวประมวลผลเบื้องหลัง (Web Worker แบบ module) ไม่ได้\nวิธีแก้: อัปเดต Chrome เป็นเวอร์ชันล่าสุด และเปิดผ่าน localhost หรือ HTTPS';
  if(code==='OOM'||e instanceof RangeError||/memory|alloc/i.test(String(e&&e.message)))return 'หน่วยความจำไม่เพียงพอสำหรับภาพขนาดนี้\nวิธีแก้: ปิดแท็บ/แอปอื่น หรือย่อภาพให้เล็กลง แล้วลองใหม่';
  if(code==='DECODE')return 'อ่านรูปไม่ได้ ไฟล์อาจเสียหรือไม่ใช่รูป JPG/PNG/WebP\nวิธีแก้: ลองบันทึกรูปใหม่หรือเลือกรูปอื่น';
  return 'ประมวลผลไม่สำเร็จ ('+(e&&e.message||e)+')\nวิธีแก้: ลองใหม่อีกครั้ง หรือเลือกโหมดโมเดล "ประหยัด"';
}

/* ---------- image loading ---------- */
async function decode(file){
  try{return await createImageBitmap(file,{colorSpaceConversion:'none'})}catch(_){}
  try{return await createImageBitmap(file)}catch(_){}
  const url=URL.createObjectURL(file);
  try{const im=new Image();im.src=url;await im.decode();return im}
  catch(_){throw new AppError('DECODE','decode failed')}
  finally{setTimeout(()=>URL.revokeObjectURL(url),1500)}
}
async function loadFile(file){
  if(!file)return;
  if(S.busy){msg('warn','กำลังประมวลผลอยู่ กรุณากด "ยกเลิก" ก่อนเปลี่ยนรูป');return}
  if(!/^image\/(jpeg|png|webp)$/.test(file.type)){msg('err','รองรับเฉพาะไฟล์ JPG, PNG และ WebP\nวิธีแก้: แปลงไฟล์เป็นรูปแบบดังกล่าวแล้วลองใหม่');return}
  clearMsg();
  try{
    const src=await decode(file);
    const W=src.naturalWidth||src.width,H=src.naturalHeight||src.height;
    if(!W||!H)throw new AppError('DECODE','empty');
    if(W*H>CFG.MAX_PX){src.close&&src.close();msg('err','รูปใหญ่เกินไป ('+W+'×'+H+' = '+(W*H/1e6).toFixed(1)+' ล้านพิกเซล) เครื่องรองรับสูงสุดประมาณ '+(CFG.MAX_PX/1e6)+' ล้านพิกเซล\nวิธีแก้: ย่อรูปก่อนแล้วลองใหม่');return}
    resetImage();
    const c=document.createElement('canvas');c.width=W;c.height=H;
    const cx=c.getContext('2d',{willReadFrequently:true});
    cx.drawImage(src,0,0);
    src.close&&src.close();
    S.orig=cx.getImageData(0,0,W,H);
    c.width=c.height=0;
    S.W=W;S.H=H;S.name=(file.name||'image').replace(/\.[^.]+$/,'');
    const d=S.orig.data;let hasA=false;
    for(let i=3;i<d.length;i+=4){if(d[i]<255){hasA=true;break}}
    if(hasA){S.origA=new Uint8Array(W*H);for(let i=0;i<W*H;i++)S.origA[i]=d[i*4+3]}
    cOrig.width=W;cOrig.height=H;cOrig.getContext('2d').putImageData(S.orig,0,0);
    cRes.width=W;cRes.height=H;
    stage.style.width=W+'px';stage.style.height=H+'px';resWrap.style.width=W+'px';resWrap.style.height=H+'px';
    stage.style.display='block';$('#empty').style.display='none';
    renderAll();applyMode();fit();
    $('#imgInfo').textContent='ต้นฉบับ: '+W+'×'+H+' px ('+(W*H/1e6).toFixed(1)+' MP) · '+fmtBytes(file.size)+(hasA?' · มีความโปร่งใสอยู่แล้ว (จะคงไว้)':'');
    if(W*H>CFG.WARN_PX)msg('warn','รูปค่อนข้างใหญ่ ('+(W*H/1e6).toFixed(1)+' ล้านพิกเซล) การประมวลผลอาจช้าหรือกินหน่วยความจำมากบนมือถือ\nถ้าค้างหรือขึ้นข้อผิดพลาด ให้ย่อรูปก่อน');
    updateUI();
  }catch(e){resetImage();msg('err',humanError(e));updateUI()}
}
function resetImage(){
  S.orig=S.origA=S.mask=S.base=null;S.hist=[];S.redo=[];S.W=S.H=0;
  cOrig.width=cOrig.height=cRes.width=cRes.height=0;
  $('#expInfo').textContent='';$('#imgInfo').textContent='';
  stage.style.display='none';$('#empty').style.display='flex';
}

/* ---------- rendering (RGB original never modified; only alpha computed) ---------- */
function alphaAt(i){const m=S.mask[i];return S.origA?((m*S.origA[i]+127)/255)|0:m}
function renderRect(x0,y0,rw,rh){
  x0=Math.max(0,x0|0);y0=Math.max(0,y0|0);
  rw=Math.min(S.W-x0,rw|0);rh=Math.min(S.H-y0,rh|0);
  if(rw<=0||rh<=0)return;
  const id=ctxRes.createImageData(rw,rh),d=id.data,o=S.orig.data,W=S.W,mode=S.mode,hasM=!!S.mask;
  for(let y=0;y<rh;y++){
    let i=(y0+y)*W+x0,k=y*rw*4;
    for(let x=0;x<rw;x++,i++,k+=4){
      const j=i*4;
      if(!hasM){d[k]=o[j];d[k+1]=o[j+1];d[k+2]=o[j+2];d[k+3]=o[j+3];continue}
      const a=alphaAt(i);
      if(mode==='mask'){d[k]=d[k+1]=d[k+2]=a;d[k+3]=255}
      else if(mode==='overlay'){const t=(255-a)/255*.6;d[k]=o[j]*(1-t)+255*t;d[k+1]=o[j+1]*(1-t)+40*t;d[k+2]=o[j+2]*(1-t)+70*t;d[k+3]=255}
      else{d[k]=o[j];d[k+1]=o[j+1];d[k+2]=o[j+2];d[k+3]=a}
    }
  }
  ctxRes.putImageData(id,x0,y0);
}
function renderAll(){for(let y=0;y<S.H;y+=256)renderRect(0,y,S.W,Math.min(256,S.H-y))}

function applyMode(){
  const m=S.mode;
  cOrig.style.display=(m==='orig'||m==='compare')?'block':'none';
  resWrap.style.display=(m==='orig')?'none':'block';
  resWrap.style.clipPath=m==='compare'?'inset(0 0 0 '+S.cmp+'%)':'none';
  divider.style.display=m==='compare'?'block':'none';
  divider.style.left=S.cmp+'%';
  $('#cmpRow').style.display=m==='compare'?'flex':'none';
  for(const b of document.querySelectorAll('#modes .btn'))b.classList.toggle('on',b.dataset.mode===m);
}
function setMode(m){const needRender=(['mask','overlay'].includes(m))!==(['mask','overlay'].includes(S.mode))||m==='mask'||m==='overlay'||S.mode==='mask'||S.mode==='overlay';S.mode=m;if(S.orig){if(needRender)renderAll();applyMode()}else{applyMode()}}
for(const b of document.querySelectorAll('#modes .btn'))b.onclick=()=>setMode(b.dataset.mode);
$('#cmp').oninput=e=>{S.cmp=+e.target.value;applyMode()};
$('#bg').onchange=e=>{resWrap.classList.remove('bg-white','bg-black','bg-green');if(e.target.value)resWrap.classList.add(e.target.value)};

/* ---------- zoom / pan ---------- */
function applyView(){
  const v=S.v;
  stage.style.transform='translate('+v.x+'px,'+v.y+'px) scale('+v.s+')';
  stage.style.setProperty('--s',v.s);resWrap.style.setProperty('--ck',(16/v.s)+'px');
  stage.classList.toggle('px',v.s*devicePixelRatio>=3);
  $('#zoomlbl').textContent=Math.round(v.s*devicePixelRatio*100)+'%';
}
function fit(){
  if(!S.orig)return;
  const r=vp.getBoundingClientRect();
  const s=Math.min(r.width/S.W,r.height/S.H)*.98;
  S.fitS=s;S.v.s=s;S.v.x=(r.width-S.W*s)/2;S.v.y=(r.height-S.H*s)/2;applyView();
}
function zoomAt(cx,cy,ns){
  ns=Math.max(S.fitS*.3,Math.min(48,ns));
  const r=vp.getBoundingClientRect(),px=cx-r.left,py=cy-r.top,v=S.v;
  v.x=px-(px-v.x)*ns/v.s;v.y=py-(py-v.y)*ns/v.s;v.s=ns;applyView();
}
function zoomCenter(f){const r=vp.getBoundingClientRect();zoomAt(r.left+r.width/2,r.top+r.height/2,S.v.s*f)}
$('#zin').onclick=()=>zoomCenter(1.5);$('#zout').onclick=()=>zoomCenter(1/1.5);
$('#zfit').onclick=fit;
$('#zreset').onclick=()=>{const r=vp.getBoundingClientRect();zoomAt(r.left+r.width/2,r.top+r.height/2,1/devicePixelRatio)};
vp.addEventListener('wheel',e=>{if(!S.orig)return;e.preventDefault();zoomAt(e.clientX,e.clientY,S.v.s*Math.exp(-e.deltaY*.0015))},{passive:false});
addEventListener('resize',()=>{if(S.orig)fit()});

/* ---------- mask editing (alpha only) ---------- */
const T=CFG.TILE;
let cur=null; // current stroke tiles
function tilesX(){return Math.ceil(S.W/T)}
function saveTiles(x0,y0,x1,y1){
  const tx=tilesX();
  for(let ty=y0>>6;ty<=y1>>6;ty++)for(let cx=x0>>6;cx<=x1>>6;cx++){
    const key=ty*tx+cx;
    if(cur.has(key))continue;
    const px=cx*T,py=ty*T,tw=Math.min(T,S.W-px),th=Math.min(T,S.H-py),buf=new Uint8Array(tw*th);
    for(let y=0;y<th;y++){const s=(py+y)*S.W+px;buf.set(S.mask.subarray(s,s+tw),y*tw)}
    cur.set(key,buf);
  }
}
function swapTiles(entry){
  const tx=tilesX();let ax0=1e9,ay0=1e9,ax1=0,ay1=0;
  for(const [key,buf] of entry){
    const cx=key%tx,ty=(key/tx)|0,px=cx*T,py=ty*T,tw=Math.min(T,S.W-px),th=Math.min(T,S.H-py);
    for(let y=0;y<th;y++){const s=(py+y)*S.W+px;for(let x=0;x<tw;x++){const t=S.mask[s+x];S.mask[s+x]=buf[y*tw+x];buf[y*tw+x]=t}}
    ax0=Math.min(ax0,px);ay0=Math.min(ay0,py);ax1=Math.max(ax1,px+tw);ay1=Math.max(ay1,py+th);
  }
  if(ax1>ax0)renderRect(ax0,ay0,ax1-ax0,ay1-ay0);
}
function undo(){const e=S.hist.pop();if(!e)return;swapTiles(e);S.redo.push(e);updateUI()}
function redo(){const e=S.redo.pop();if(!e)return;swapTiles(e);S.hist.push(e);updateUI()}
$('#undo').onclick=undo;$('#redo').onclick=redo;
$('#resetMask').onclick=()=>{
  if(!S.mask||!confirm('คืนหน้ากากกลับเป็นผลการประมวลผลครั้งแรก? (ประวัติ Undo จะถูกล้าง)'))return;
  S.mask.set(S.base);S.hist=[];S.redo=[];renderAll();updateUI();
};
addEventListener('keydown',e=>{
  if((e.ctrlKey||e.metaKey)&&e.key.toLowerCase()==='z'){e.preventDefault();e.shiftKey?redo():undo()}
  else if((e.ctrlKey||e.metaKey)&&e.key.toLowerCase()==='y'){e.preventDefault();redo()}
});

let dirty=null;
function markDirty(x0,y0,x1,y1){if(!dirty)dirty=[x0,y0,x1,y1];else{dirty[0]=Math.min(dirty[0],x0);dirty[1]=Math.min(dirty[1],y0);dirty[2]=Math.max(dirty[2],x1);dirty[3]=Math.max(dirty[3],y1)}}
function flushDirty(){if(!dirty)return;renderRect(dirty[0],dirty[1],dirty[2]-dirty[0]+1,dirty[3]-dirty[1]+1);dirty=null}
function stamp(cx,cy,r,soft,restore){
  const W=S.W,H=S.H;
  const x0=Math.max(0,Math.floor(cx-r)),x1=Math.min(W-1,Math.ceil(cx+r)),y0=Math.max(0,Math.floor(cy-r)),y1=Math.min(H-1,Math.ceil(cy+r));
  if(x1<x0||y1<y0)return;
  saveTiles(x0,y0,x1,y1);
  const hard=1-soft,r2=r*r,m=S.mask;
  for(let y=y0;y<=y1;y++){
    const dy=y-cy;
    for(let x=x0;x<=x1;x++){
      const dx=x-cx,d2=dx*dx+dy*dy;
      if(d2>r2)continue;
      let s=1;
      if(soft>0){const t=(Math.sqrt(d2)/r-hard)/(soft);s=t<=0?1:1-t;s=s*s*(3-2*s)}
      if(s<=0)continue;
      const i=y*W+x,a=m[i];
      m[i]=restore?Math.round(a+(255-a)*s):Math.round(a*(1-s));
    }
  }
  markDirty(x0,y0,x1,y1);
}
let stroke=null;
function toImg(cx,cy){const r=vp.getBoundingClientRect();return [(cx-r.left-S.v.x)/S.v.s,(cy-r.top-S.v.y)/S.v.s]}
function brushR(){return (+$('#bsize').value/2)/S.v.s}
function strokeTo(px,py){
  const r=brushR(),soft=(+$('#bsoft').value)/100,restore=S.tool==='restore';
  const [lx,ly]=stroke.last,dx=px-lx,dy=py-ly,dist=Math.hypot(dx,dy),step=Math.max(1,r*.25),n=Math.max(1,Math.ceil(dist/step));
  for(let k=1;k<=n;k++)stamp(lx+dx*k/n,ly+dy*k/n,r,soft,restore);
  stroke.last=[px,py];flushDirty();
}
function startStroke(e){
  cur=new Map();stroke={last:null};
  const [x,y]=toImg(e.clientX,e.clientY);stroke.last=[x,y];
  stamp(x,y,brushR(),(+$('#bsoft').value)/100,S.tool==='restore');flushDirty();
}
function endStroke(){
  if(!stroke)return;
  if(cur&&cur.size){S.hist.push(cur);if(S.hist.length>CFG.HIST)S.hist.shift();S.redo=[]}
  cur=null;stroke=null;updateUI();
}
$('#bsize').oninput=e=>{$('#bsizeV').textContent=e.target.value};
$('#bsoft').oninput=e=>{$('#bsoftV').textContent=e.target.value};
for(const b of document.querySelectorAll('#tools .btn'))b.onclick=()=>{
  if(b.disabled)return;
  S.tool=b.dataset.tool;
  for(const x of document.querySelectorAll('#tools .btn'))x.classList.toggle('on',x===b);
  if(S.tool!=='pan'&&(S.mode==='orig'))setMode('result');
  cursor.style.display='none';
};

/* ---------- pointer handling ---------- */
const ptrs=new Map();let pinch=null,pan=null;
function startPan(p){pan={sx:p.x,sy:p.y,x:S.v.x,y:S.v.y}}
vp.addEventListener('pointerdown',e=>{
  if(!S.orig)return;
  try{vp.setPointerCapture(e.pointerId)}catch(_){}
  ptrs.set(e.pointerId,{x:e.clientX,y:e.clientY});
  if(ptrs.size===2){
    endStroke();pan=null;
    const [a,b]=[...ptrs.values()];
    pinch={d:Math.hypot(a.x-b.x,a.y-b.y)||1,cx:(a.x+b.x)/2,cy:(a.y+b.y)/2,s:S.v.s,x:S.v.x,y:S.v.y};
  }else if(ptrs.size===1){
    if(S.tool==='pan'||!S.mask||S.busy)startPan({x:e.clientX,y:e.clientY});
    else startStroke(e);
  }
});
vp.addEventListener('pointermove',e=>{
  if(S.orig&&S.mask&&S.tool!=='pan'&&e.pointerType!=='touch'){
    const r=vp.getBoundingClientRect(),sz=+$('#bsize').value;
    cursor.style.display='block';cursor.style.width=cursor.style.height=sz+'px';
    cursor.style.left=(e.clientX-r.left)+'px';cursor.style.top=(e.clientY-r.top)+'px';
  }else cursor.style.display='none';
  if(!ptrs.has(e.pointerId))return;
  ptrs.set(e.pointerId,{x:e.clientX,y:e.clientY});
  if(pinch&&ptrs.size>=2){
    const [a,b]=[...ptrs.values()],d=Math.hypot(a.x-b.x,a.y-b.y)||1,cx=(a.x+b.x)/2,cy=(a.y+b.y)/2;
    const ns=Math.max(S.fitS*.3,Math.min(48,pinch.s*d/pinch.d)),r=vp.getBoundingClientRect();
    const p0x=(pinch.cx-r.left-pinch.x)/pinch.s,p0y=(pinch.cy-r.top-pinch.y)/pinch.s;
    S.v.s=ns;S.v.x=(cx-r.left)-p0x*ns;S.v.y=(cy-r.top)-p0y*ns;applyView();
  }else if(stroke){
    const evs=e.getCoalescedEvents?e.getCoalescedEvents():[e];
    for(const ce of (evs.length?evs:[e])){const [x,y]=toImg(ce.clientX,ce.clientY);strokeTo(x,y)}
  }else if(pan){
    S.v.x=pan.x+(e.clientX-pan.sx);S.v.y=pan.y+(e.clientY-pan.sy);applyView();
  }
});
function ptrEnd(e){
  if(!ptrs.has(e.pointerId))return;
  ptrs.delete(e.pointerId);
  if(ptrs.size<2)pinch=null;
  if(ptrs.size===0){endStroke();pan=null}
  else if(ptrs.size===1&&!stroke){const p=[...ptrs.values()][0];startPan(p)}
}
vp.addEventListener('pointerup',ptrEnd);vp.addEventListener('pointercancel',ptrEnd);
vp.addEventListener('pointerleave',()=>{cursor.style.display='none'});

/* ---------- worker / inference ---------- */
async function detectGPU(){
  try{if(!navigator.gpu)return false;return !!(await navigator.gpu.requestAdapter())}catch(_){return false}
}
function onWorkerMsg(e){
  const m=e.data;
  if(m.type==='progress')setProgress(m.pct,m.text);
  else if(m.type==='ready'){S.ready=true;S.backend=m.backend;$('#chipBackend').textContent='โมเดลพร้อม: '+m.backend;const p=S.pending.init;S.pending.init=null;p&&p.res()}
  else if(m.type==='backend'){S.backend=m.backend;$('#chipBackend').textContent='โมเดลพร้อม: '+m.backend}
  else if(m.type==='done'){const p=S.pending.run;S.pending.run=null;p&&p.res(m.buf)}
  else if(m.type==='error'){
    const err=new AppError(m.code,m.message);
    if(m.id!==undefined&&S.pending.run){const p=S.pending.run;S.pending.run=null;p.rej(err)}
    else if(S.pending.init){const p=S.pending.init;S.pending.init=null;killWorker();p.rej(err)}
  }
}
function killWorker(){
  if(S.worker){S.worker.terminate();S.worker=null}
  S.ready=false;$('#chipBackend').textContent='ยังไม่โหลดโมเดล';
}
function startWorker(){
  return new Promise(async(res,rej)=>{
    try{
      const hasGPU=await detectGPU();
      const url=URL.createObjectURL(new Blob([$('#workerSrc').textContent],{type:'text/javascript'}));
      const w=new Worker(url,{type:'module'});
      S.worker=w;
      w.onmessage=onWorkerMsg;
      w.onerror=ev=>{
        const err=new AppError('WORKER',ev.message||'worker error');
        for(const k of ['init','run']){const p=S.pending[k];S.pending[k]=null;p&&p.rej(err)}
        killWorker();
      };
      S.pending.init={res,rej};
      w.postMessage({type:'init',lib:CFG.LIB,model:CFG.MODEL,hasGPU,quality:$('#quality').value});
    }catch(e){rej(new AppError('WORKER',e.message))}
  });
}
async function ensureWorker(){
  if(S.ready)return;
  if(!S.initP)S.initP=startWorker().finally(()=>{S.initP=null});
  return S.initP;
}
$('#quality').onchange=()=>{if(S.busy)return;killWorker()}; // เปลี่ยนโหมดต้องโหลดโมเดลใหม่

function inferOnWorker(buf){
  return new Promise((res,rej)=>{S.pending.run={res,rej};S.worker.postMessage({type:'run',id:1,buf},[buf])});
}
function buildInput(){
  const N=1024,c=document.createElement('canvas');c.width=c.height=N;
  const cx=c.getContext('2d',{willReadFrequently:true});
  cx.fillStyle='#fff';cx.fillRect(0,0,N,N);
  cx.imageSmoothingEnabled=true;cx.imageSmoothingQuality='high';
  cx.drawImage(cOrig,0,0,N,N);
  const px=cx.getImageData(0,0,N,N).data;c.width=c.height=0;
  return px.buffer;
}
function upscaleMask(buf){
  const W=S.W,H=S.H,N=1024;
  const small=document.createElement('canvas');small.width=small.height=N;
  const sc=small.getContext('2d'),sid=sc.createImageData(N,N),sd=sid.data,m=new Uint8ClampedArray(buf);
  for(let i=0;i<N*N;i++){sd[i*4]=sd[i*4+1]=sd[i*4+2]=255;sd[i*4+3]=m[i]}
  sc.putImageData(sid,0,0);
  const out=new Uint8Array(W*H),strip=256,sk=document.createElement('canvas');sk.width=W;sk.height=strip;
  const kc=sk.getContext('2d',{willReadFrequently:true});
  for(let y0=0;y0<H;y0+=strip){
    const h=Math.min(strip,H-y0);
    kc.setTransform(1,0,0,1,0,0);kc.clearRect(0,0,W,strip);
    kc.imageSmoothingEnabled=true;kc.imageSmoothingQuality='high';
    kc.setTransform(W/N,0,0,H/N,0,-y0);kc.drawImage(small,0,0);
    const d=kc.getImageData(0,0,W,h).data;
    for(let i=0,o=y0*W;i<W*h;i++,o++)out[o]=d[i*4+3];
  }
  small.width=small.height=0;sk.width=sk.height=0;
  return out;
}
async function runRemoval(){
  if(!S.orig||S.busy)return;
  clearMsg();S.busy=true;updateUI();setMode(S.mode==='orig'?'result':S.mode);
  try{
    if(!S.ready)setProgress(null,'ครั้งแรกต้องดาวน์โหลดไลบรารีและโมเดล (≈44–176 MB) ต้องใช้อินเทอร์เน็ต');
    await ensureWorker();
    setProgress(null,'กำลังวิเคราะห์ภาพ…');
    await new Promise(r=>setTimeout(r,30));
    const input=buildInput();
    const maskBuf=await inferOnWorker(input);
    setProgress(null,'กำลังปรับหน้ากากให้ตรงความละเอียดเดิม…');
    await new Promise(r=>setTimeout(r,30));
    S.mask=upscaleMask(maskBuf);S.base=S.mask.slice();S.hist=[];S.redo=[];
    renderAll();applyMode();
    let tr=0;const n=S.W*S.H;for(let i=0;i<n;i+=7)if(alphaAt(i)<128)tr++;
    if(tr/(n/7)<.001)msg('warn','ไม่พบพื้นหลังที่ถูกลบเลย (ภาพอาจไม่มีพื้นหลังชัดเจน) ลองใช้ Eraser ลบส่วนที่ต้องการเอง');
    else if(tr/(n/7)>.97)msg('warn','พื้นที่เกือบทั้งภาพถูกลบ ตรวจสอบด้วยมุมมอง "พื้นที่ที่ลบ" แล้วใช้ Brush คืนวัตถุได้');
  }catch(e){
    if(e&&e.code==='ABORT')msg('info',humanError(e));else msg('err',humanError(e));
    if(e&&(e.code==='INFER'||e.code==='OOM'))killWorker();
  }finally{S.busy=false;S.pending.run=null;hideProgress();updateUI()}
}
$('#run').onclick=runRemoval;
$('#cancel').onclick=()=>{
  if(!S.busy)return;
  const err=new AppError('ABORT','cancelled');
  for(const k of ['init','run']){const p=S.pending[k];S.pending[k]=null;p&&p.rej(err)}
  killWorker();
};

/* ---------- export: PNG encoder keeps original RGB, writes alpha ---------- */
const CRC=(()=>{const t=new Uint32Array(256);for(let n=0;n<256;n++){let c=n;for(let k=0;k<8;k++)c=c&1?0xEDB88320^(c>>>1):c>>>1;t[n]=c>>>0}return t})();
function crc32(b){let c=0xFFFFFFFF;for(let i=0;i<b.length;i++)c=CRC[(c^b[i])&255]^(c>>>8);return (c^0xFFFFFFFF)>>>0}
function chunk(type,data){
  const out=new Uint8Array(12+data.length),dv=new DataView(out.buffer);
  dv.setUint32(0,data.length);
  for(let i=0;i<4;i++)out[4+i]=type.charCodeAt(i);
  out.set(data,8);dv.setUint32(8+data.length,crc32(out.subarray(4,8+data.length)));
  return out;
}
function nearestOpaque(x,y,R){
  const W=S.W,H=S.H;let best=-1,bd=1e9;
  for(let dy=-R;dy<=R;dy++){const yy=y+dy;if(yy<0||yy>=H)continue;
    for(let dx=-R;dx<=R;dx++){const xx=x+dx;if(xx<0||xx>=W)continue;
      const i=yy*W+xx;if(alphaAt(i)>=250){const d=dx*dx+dy*dy;if(d<bd){bd=d;best=i}}}}
  return best;
}
function buildRow(y,row,decon){
  const W=S.W,o=S.orig.data;
  for(let x=0;x<W;x++){
    const i=y*W+x,j=i*4,a=alphaAt(i);
    let r=o[j],g=o[j+1],b=o[j+2];
    if(decon&&a>0&&a<250){
      const n=nearestOpaque(x,y,4);
      if(n>=0){const t=1-a/255,q=n*4;r=Math.round(r+(o[q]-r)*t);g=Math.round(g+(o[q+1]-g)*t);b=Math.round(b+(o[q+2]-b)*t)}
    }
    const k=x*4;row[k]=r;row[k+1]=g;row[k+2]=b;row[k+3]=a;
  }
}
async function encodePNG(decon,onProg){
  const W=S.W,H=S.H,stride=W*4;
  if(typeof CompressionStream==='undefined'){
    const c=document.createElement('canvas');c.width=W;c.height=H;
    const id=new ImageData(W,H),row=new Uint8Array(stride);
    for(let y=0;y<H;y++){buildRow(y,row,decon);id.data.set(row,y*stride);if(y%128===0){onProg(y/H);await new Promise(r=>setTimeout(r))}}
    c.getContext('2d').putImageData(id,0,0);
    const blob=await new Promise(r=>c.toBlob(r,'image/png'));
    c.width=c.height=0;
    if(!blob)throw new AppError('OOM','toBlob failed');
    return {blob,fallback:true};
  }
  const raw=new Uint8Array((stride+1)*H),row=new Uint8Array(stride);
  for(let y=0;y<H;y++){
    buildRow(y,row,decon);
    const base=y*(stride+1);raw[base]=1; // filter: Sub
    for(let k=0;k<stride;k++)raw[base+1+k]=(row[k]-(k>=4?row[k-4]:0))&255;
    if(y%64===0){onProg(y/H);await new Promise(r=>setTimeout(r))}
  }
  const z=new Uint8Array(await new Response(new Blob([raw]).stream().pipeThrough(new CompressionStream('deflate'))).arrayBuffer());
  const ihdr=new Uint8Array(13),dv=new DataView(ihdr.buffer);
  dv.setUint32(0,W);dv.setUint32(4,H);ihdr[8]=8;ihdr[9]=6;ihdr[10]=0;ihdr[11]=0;ihdr[12]=0;
  const sig=new Uint8Array([137,80,78,71,13,10,26,10]);
  return {blob:new Blob([sig,chunk('IHDR',ihdr),chunk('IDAT',z),chunk('IEND',new Uint8Array(0))],{type:'image/png'}),fallback:false};
}
$('#dl').onclick=async()=>{
  if(!S.mask||S.exporting||S.busy)return;
  clearMsg();S.exporting=true;updateUI();
  try{
    const {blob,fallback}=await encodePNG($('#decon').checked,p=>setProgress(p*100,'กำลังสร้างไฟล์ PNG ความละเอียดเต็ม…'));
    const name=S.name+'_nobg.png',url=URL.createObjectURL(blob),a=document.createElement('a');
    a.href=url;a.download=name;document.body.appendChild(a);a.click();a.remove();
    setTimeout(()=>URL.revokeObjectURL(url),30000);
    $('#expInfo').textContent='ส่งออก: '+name+' · '+S.W+'×'+S.H+' px · '+fmtBytes(blob.size)+' · PNG RGBA (มี Alpha Channel)';
    if(fallback)msg('warn','เบราว์เซอร์ไม่รองรับตัวเข้ารหัส PNG แบบเต็ม จึงใช้ตัวเข้ารหัสของ Canvas แทน: สี RGB ในพื้นที่โปร่งใสบางส่วนอาจไม่ตรงต้นฉบับ (พื้นที่ทึบยังตรง)');
  }catch(e){msg('err','ดาวน์โหลดไม่สำเร็จ: '+(e.code==='OOM'||e instanceof RangeError?'หน่วยความจำไม่พอสำหรับสร้างไฟล์ขนาดนี้ ปิดแท็บอื่นหรือย่อรูปแล้วลองใหม่':'ลองกดดาวน์โหลดอีกครั้ง หากยังไม่ได้ ให้ตรวจสิทธิ์การดาวน์โหลดของเบราว์เซอร์'))}
  finally{S.exporting=false;hideProgress();updateUI()}
};

/* ---------- input wiring ---------- */
$('#pick').onclick=()=>$('#file').click();
$('#file').onchange=e=>{const f=e.target.files[0];e.target.value='';loadFile(f)};
const drop=$('#drop');
for(const t of ['dragenter','dragover'])addEventListener(t,e=>{e.preventDefault();drop.classList.add('over')});
for(const t of ['dragleave','drop'])addEventListener(t,e=>{e.preventDefault();drop.classList.remove('over')});
addEventListener('drop',e=>{const f=e.dataTransfer&&e.dataTransfer.files[0];if(f)loadFile(f)});
addEventListener('paste',e=>{
  const items=e.clipboardData&&e.clipboardData.files;
  if(items&&items.length){loadFile(items[0])}
});
$('#pasteBtn').onclick=async()=>{
  try{
    if(!navigator.clipboard||!navigator.clipboard.read)throw 0;
    const its=await navigator.clipboard.read();
    for(const it of its){const t=it.types.find(x=>/^image\/(png|jpeg|webp)$/.test(x));if(t){const b=await it.getType(t);return loadFile(new File([b],'clipboard.'+t.split('/')[1],{type:t}))}}
    msg('warn','ไม่พบรูปในคลิปบอร์ด');
  }catch(_){msg('warn','เบราว์เซอร์ไม่อนุญาตหรือไม่รองรับการอ่านคลิปบอร์ดโดยตรง\nวิธีแก้: กดค้างในหน้านี้แล้วเลือก "วาง" หรือใช้ปุ่มเลือกรูปแทน')}
};
applyMode();applyView();updateUI();
</script>
</body>
</html>
