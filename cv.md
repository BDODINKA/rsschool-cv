# Hi,My name is Dmitry #
![](../../Desktop/1.jpg)
### I'm learning to FrontEnd Developer ###
#### Contacts ####
[Github](https://github.com/BDODINKA)
[Gmail](https://bdodinka1992@gmail.com)
#### Links CV ####
[CV]()

#### Skills ####                          
- [x] HTML
- [x] CSS
- [x] Basic JS
- [x] Figma
- [x] Basic adobe Photoshop
#### Skills on future learning ####
- [ ] Sass/Less
- [ ] WebPack/Gulp
- [ ] React JS
- [ ] Angular JS
- [ ] Vue JS
- [ ] Redux/Redux-saga/MobX
- [ ] Node Js
#### Experience ####
* RS-School Stage 0 *
#### Education #### 
* Belarussian State University of Informatics and RadioElectronics *
#### Languages ####
* A1-A2-*

```//search btn
const btnPrev = document.querySelector(".btn-prev");
const btnNext = document.querySelector(".btn-next");
const slideImg = document.querySelector('.slide-img');

//event listener btn
btnPrev.addEventListener('click', onPrevClick);
btnNext.addEventListener('click', onNextClick);

//array add img
const imgAll = [];
imgAll.push(src="/slider/img/1.jpeg");
imgAll.push(src="/slider/img/2.jpeg");
imgAll.push(src="/slider/img/3.jpeg");
imgAll.push(src="/slider/img/4.jpeg");
imgAll.push(src="/slider/img/5.jpeg");

//Show img start
let currentImageIndex = 0;
slideImg.src = imgAll[currentImageIndex];
btnPrev.disabled = true;

//function btn
function onPrevClick(){
    currentImageIndex --;
    slideImg.src = imgAll[currentImageIndex];
    btnNext.disabled = false;
    if(currentImageIndex === 0){
        btnPrev.disabled = true;
    };
};

function onNextClick(){
    currentImageIndex ++;
    slideImg.src = imgAll[currentImageIndex];
    btnPrev.disabled = false;
    if(currentImageIndex === (imgAll.length -1)){
        btnNext.disabled = true;
    };
};
```
