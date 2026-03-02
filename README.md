<section style="padding:60px 20px;text-align:center;background:#fff">
<h2 style="margin-bottom:30px">معرض أعمالنا</h2>

<div class="gallery">

<img src="https://images.unsplash.com/photo-1598902108854-10e335adac99" onclick="openModal(this.src)">
<img src="https://images.unsplash.com/photo-1600585154340-be6161a56a0c" onclick="openModal(this.src)">
<img src="https://images.unsplash.com/photo-1600607687939-ce8a6c25118c" onclick="openModal(this.src)">
<img src="https://images.unsplash.com/photo-1501004318641-b39e6451bec6" onclick="openModal(this.src)">
<img src="https://images.unsplash.com/photo-1502086223501-7ea6ecd79368" onclick="openModal(this.src)">
<img src="https://images.unsplash.com/photo-1560185127-6ed189bf02f4" onclick="openModal(this.src)">

</div>
</section>

<!-- نافذة تكبير الصور -->
<div id="modal" onclick="closeModal()" style="
display:none;
position:fixed;
top:0;left:0;
width:100%;height:100%;
background:rgba(0,0,0,0.9);
justify-content:center;
align-items:center;
z-index:999;
">
<img id="modalImg" style="max-width:90%;max-height:90%;border-radius:10px">
</div>

<style>
.gallery{
display:grid;
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
gap:15px;
}

.gallery img{
width:100%;
border-radius:12px;
cursor:pointer;
transition:.4s;
}

.gallery img:hover{
transform:scale(1.05);
}
</style>

<script>
function openModal(src){
document.getElementById("modal").style.display="flex";
document.getElementById("modalImg").src=src;
}

function closeModal(){
document.getElementById("modal").style.display="none";
}
</script>
