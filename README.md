/* MENU MOBILE */
const hamburger = document.getElementById("hamburger");
const menu = document.getElementById("menu");

hamburger.addEventListener("click", () => {
menu.classList.toggle("active");
});

/* ANIMATION SCROLL */
function reveal() {
const reveals = document.querySelectorAll(".reveal");

reveals.forEach(element => {
const windowHeight = window.innerHeight;
const elementTop = element.getBoundingClientRect().top;

if(elementTop < windowHeight - 100){
element.classList.add("active");
}
});
}

window.addEventListener("scroll", reveal);
