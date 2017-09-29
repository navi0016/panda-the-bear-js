var profilePic = document.querySelector('img')
profilePic.setAttribute('src','images/self-portrait-snowbg.jpg')

var photoPic = document.querySelectorAll('img')
photoPic[1].setAttribute('src','http://media.istockphoto.com/vectors/beautiful-woman-vector-logo-template-vector-id655503002')
photoPic[1].style.width = '325px'
photoPic[1].style.height = '225px'


var title = document.querySelector('h1')
title.innerText = 'Navi'

var educationTitle = document.querySelectorAll('h3')
educationTitle[1].innerText = "you are now Something Else"

document.body.style.backgroundColor = 'red'

var highlight = document.body.querySelectorAll('.highlight')
  for (var i = 0; i < highlight.length; i ++) {
    highlight[i].style.color = 'yellow';
  }

var newFontH1 = document.body.querySelector('h1')  
  newFontH1.style.fontFamily = 'monospace'

var roundIcons = document.body.querySelectorAll('.action-icon-bg')
for (var i = 0; i < roundIcons.length; i ++) {
  roundIcons[i].style.background = 'purple';
}

var giveName = document.querySelector('#name')
giveName.setAttribute('placeholder','identify yourself')

var giveMsg = document.querySelector('#message')
giveMsg.setAttribute('placeholder','state your business')

var giveName = document.querySelector('#name')
giveName.setAttribute('value','your nemesis')

var giveEmail = document.querySelector('#email')
giveEmail.setAttribute('value','koalathebear@gmail.com')

var hitSubmit = document.querySelector('#submit')
hitSubmit.setAttribute('value','En garde!')

hitSubmit.disabled = true;

var personalInfo = document.querySelector('.bio-info')
personalInfo.innerHTML = null

var timeTravel = document.querySelectorAll('.bar-default')
timeTravel[2].outerHTML = null

---------------------------------------
<!-- crete a clone of pickachuPic under portfolioContainer -->

var pickachuPic = document.querySelectorAll('img')
var copyPickachu = pickachuPic[2].cloneNode(true)
var portfolioContainer = document.querySelector('.portfolio-container')
var portfolioContainer = document.querySelector('.portfolio-container')
portfolioContainer.appendChild(copyPickachu)

-------------------------------------
<!-- copy pickachuPic 10 times using loop -->
var pickachuPic = document.querySelectorAll('img')
var portfolioContainer = document.querySelector('.portfolio-container')
for ( i = 0; i < 10; i++) {
    var copyPickachu = pickachuPic[2].cloneNode(true)
    portfolioContainer.appendChild(copyPickachu)
}

--------------------------------------
<!-- add a message about when the page was last updated  -->
var bioInfo = document.querySelector('.bio-info')
var listItem = document.createElement('li')
var leftSpan = document.createElement('span')
var lastUpdated = document.createTextNode('Page last updated on')
leftSpan.appendChild(lastUpdated)
listItem.appendChild(leftSpan)
bioInfo.appendChild(listItem)
<!-- give new li a class name -->
var nameClass = document.querySelectorAll('li')
nameClass[3].setAttribute('class','bio-info-item')

----------------------------------
<!-- adding date -->
var rightSpan = document.createElement('span')
var updatedAt = new Date()
rightSpan.innerHTML = updatedAt
var nameClass = document.querySelectorAll('.bio-info-item')
nameClass[3].appendChild(rightSpan)
