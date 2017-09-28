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
