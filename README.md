# Google-Dino-Cheat

想要运行作弊代码，有两种方法。

1. 书签法

在浏览器创建一个新书签，名称随便，URL为这个：

```
javascript:%22use%20strict%22;void%20function($){var%20loadBookmarklet=function($){function%20cheat(){const%20mode=prompt(%22\u4F5C\u5F0A\u83DC\u5355\n1:\u65E0\u654C\n2:\u5954\u8DD1\u901F\u5EA6\u4FEE\u6539\n3:\u8DF3\u8DC3\u9AD8\u5EA6\u4FEE\u6539\n4:\u6539\u5199\u8BA1\u5206\u903B\u8F91\n5:\u81EA\u52A8\u64CD\u4F5C\n6:\u539F\u5730\u8E0F\u6B65\n7:\u9000\u51FA%22);if(%221%22===mode){var%20of=confirm(%22\u662F\u5426\u5F00\u542F\u65E0\u654C\u6A21\u5F0F\uFF1F%22);of%3F(Runner.instance_.gameOver=function(){},alert(%22\u65E0\u654C\u6A21\u5F0F\u5DF2\u5F00\u542F%22),console.log(%22\u65E0\u654C\u6A21\u5F0F\u5DF2\u5F00\u542F%22)):(Runner.instance_.gameOver=function(){if(this.playSound(this.soundFx.HIT),vibrate(200),this.stop(),this.crashed=!0,this.distanceMeter.achievement=!1,this.tRex.update(100,Trex.status.CRASHED),!this.gameOverPanel){const%20origSpriteDef=IS_HIDPI%3FspriteDefinitionByType.original.HDPI:spriteDefinitionByType.original.LDPI;this.canvas%26%26(Runner.isAltGameModeEnabled%3Fthis.gameOverPanel=new%20GameOverPanel(this.canvas,origSpriteDef.TEXT_SPRITE,origSpriteDef.RESTART,this.dimensions,origSpriteDef.ALT_GAME_END,this.altGameModeActive):this.gameOverPanel=new%20GameOverPanel(this.canvas,origSpriteDef.TEXT_SPRITE,origSpriteDef.RESTART,this.dimensions))}this.gameOverPanel.draw(this.altGameModeActive,this.tRex),this.distanceRan%3Ethis.highestScore%26%26this.saveHighScore(this.distanceRan),this.time=getTimeStamp(),Runner.audioCues%26%26(this.generatedSoundFx.stopAll(),announcePhrase(getA11yString(A11Y_STRINGS.gameOver).replace(%22$1%22,this.distanceMeter.getActualDistance(this.distanceRan).toString())+%22%20%22+getA11yString(A11Y_STRINGS.highScore).replace(%22$1%22,this.distanceMeter.getActualDistance(this.highestScore).toString())),this.containerEl.setAttribute(%22title%22,getA11yString(A11Y_STRINGS.ariaLabel))),this.showSpeedToggle(),this.disableSpeedToggle(!1)},alert(%22\u65E0\u654C\u6A21\u5F0F\u5DF2\u5173\u95ED%22),console.log(%22\u65E0\u654C\u6A21\u5F0F\u5DF2\u5173\u95ED%22))}else%20if(%222%22===mode){var%20set_speed=parseInt(prompt(%22\u8BF7\u8F93\u5165\u8981\u4FEE\u6539\u7684\u901F\u5EA6(\u9ED8\u8BA4\u662F10)%22));Runner.instance_.setSpeed(set_speed),alert(`%E9%80%9F%E5%BA%A6%E5%B7%B2%E4%BF%AE%E6%94%B9%E4%B8%BA${set_speed}`),console.log(`%E9%80%9F%E5%BA%A6%E5%B7%B2%E4%BF%AE%E6%94%B9%E4%B8%BA${set_speed}`)}else%20if(%223%22===mode){var%20set_jump=parseInt(prompt(%22\u8BF7\u8F93\u5165\u8981\u4FEE\u6539\u7684\u8DF3\u8DC3\u9AD8\u5EA6(\u9ED8\u8BA4\u662F10)%22));Runner.instance_.tRex.setJumpVelocity(set_jump),alert(`%E8%B7%B3%E8%B7%83%E9%AB%98%E5%BA%A6%E5%B7%B2%E4%BF%AE%E6%94%B9%E4%B8%BA${set_jump}`),console.log(`%E8%B7%B3%E8%B7%83%E9%AB%98%E5%BA%A6%E5%B7%B2%E4%BF%AE%E6%94%B9%E4%B8%BA${set_jump}`)}else%20if(%224%22===mode){var%20change_score_rule=parseInt(prompt(%22\u6539\u5199\u8BA1\u5206\u903B\u8F91,\u6BD4\u4F8B\u4E3A1\uFF1A\u4F60\u8F93\u5165\u7684\u6570\u5B57\uFF0C\u5982\u679C\u8F93\u5165\u4E3A1000\uFF0C\u90A3\u4E48\u83B7\u53D6\u7684\u5206\u6570\u4E3A\u539F\u6765\u7684\u4E00\u5343\u500D(\u9ED8\u8BA4\u662F0)%22)),hackScore=0;Object.defineProperty(Runner.instance_,%22distanceRan%22,{get:()=%3EhackScore,set:value=%3EhackScore=value+Math.floor(Math.random()*change_score_rule),configurable:!0,enumerable:!0}),alert(`%E7%9B%AE%E5%89%8D%E8%AE%A1%E5%88%86%E9%80%BB%E8%BE%91%E4%B8%BA%E5%8E%9F%E6%9D%A5%E7%9A%84${change_score_rule}%E5%80%8D`),console.log(`%E7%9B%AE%E5%89%8D%E8%AE%A1%E5%88%86%E9%80%BB%E8%BE%91%E4%B8%BA%E5%8E%9F%E6%9D%A5%E7%9A%84${change_score_rule}%E5%80%8D`)}else%20if(%225%22===mode){function%20dinoAI(){if(!stopDinoAI){if(0%3CRunner.instance_.horizon.obstacles.length){let%20dist=Runner.instance_.horizon.obstacles[0].xPos,obj=Runner.instance_.horizon.obstacles[0],type=obj.typeConfig.type,speed=Runner.instance_.currentSpeed;dist%3C22*speed%26%26(%22PTERODACTYL%22===type%26%2660%3Eobj.yPos%3F!Runner.instance_.tRex.ducking%26%26Runner.instance_.tRex.setDuck(!0):(Runner.instance_.tRex.ducking%26%26Runner.instance_.tRex.setDuck(!1),Runner.instance_.tRex.startJump(Runner.instance_.currentSpeed)))}requestAnimationFrame(dinoAI)}}function%20stopAI(){stopDinoAI=!0}let%20stopDinoAI=!1;dinoAI(),alert(%22\u81EA\u52A8\u64CD\u4F5C\u5DF2\u542F\u52A8\uFF0C\u6309\u4E0B\%22s\%22\u952E\u505C\u6B62\u81EA\u52A8\u64CD\u4F5C%22),document.addEventListener(%22keydown%22,function(e){%22s%22===e.key%26%26!0==confirm(%22\u786E\u5B9A\u8981\u5173\u95ED\u81EA\u52A8\u64CD\u4F5C\u5417\uFF1F%22)%26%26stopAI()})}else%20if(%226%22==mode)!0==confirm(%22\u662F\u5426\u5F00\u542F\u539F\u5730\u8E0F\u6B65\uFF1F%22)%3F(Runner.instance_.playingIntro=!0,alert(%22\u539F\u5730\u8E0F\u6B65\u5DF2\u5F00\u542F%22),console.log(%22\u539F\u5730\u8E0F\u6B65\u5DF2\u5F00\u542F%22)):(Runner.instance_.playingIntro=!1,alert(%22\u539F\u5730\u8E0F\u6B65\u5DF2\u5173\u95ED%22),console.log(%22\u539F\u5730\u8E0F\u6B65\u5DF2\u5173\u95ED%22));else{if(%227%22==mode)return;alert(%22\u8F93\u5165\u9519\u8BEF\uFF01%22)}cheat()}document.addEventListener(%22keydown%22,function(e){%22c%22===e.key%26%26cheat()}),alert(%22\u6309\u4E0B\%22c\%22\u952E\u6765\u6253\u5F00\u4F5C\u5F0A\u83DC\u5355%22)};if($%26%26$.fn%26%261.7%3C=parseFloat($.fn.jquery))return%20void%20load($);var%20s=document.createElement(%22script%22);s.src=%22https://ajax.googleapis.com/ajax/libs/jquery/1/jquery.js%22,s.onload=s.onreadystatechange=function(){var%20state=this.readyState;state%26%26%22loaded%22!==state%26%26%22complete%22!==state||loadBookmarklet(jQuery.noConflict())},document.getElementsByTagName(%22head%22)[0].appendChild(s)}(window.jQuery);
```
注：此法不能再chrome://dino运行，可以使用第二种方法。
2. 控制台法
- 在浏览器中打开开发者工具,一般按下`F12`或`Ctrl+Shift+i`键，如果不行，点击浏览器右上角头像旁的三个点，在更多工具中可以找到它。
- 打开开发者工具后点击控制台或console。
- 在控制台中输入
```
javascript
```
在`Google-Dino`中的文件是游戏主体文件。
