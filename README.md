## Whatsapp-spam-bot-send-messages-on-loop

### Steps to send whatsapp messages on loop: -

1. Open Whatsapp web.
1. Click on the person you want to send messages on loop.
1. then open the browser console.
1. copy the code from below.
1. paste the code in browser console.
1. Hit enter then it will ask you to type your message and the number of times you want to send the message.
1. Done. 👍


# NOTE: there are two class names that are keep on changing, so if this code throws any error then just inspect the textbox of whatsapp and change the class name accoring to that in 5th line of code. and same for send button in 9th line.

```javascript
-------------------------------------------------------------------------------------------------------
var message = prompt("Enter your message", "‎");
var counter = parseInt(prompt("How many Times ?", 10));
window.InputEvent = window.Event || window.InputEvent;
var event = new InputEvent("input", { bubbles: true });
var textbox = document.getElementsByClassName("_13NKt copyable-text selectable-text")[1];
for (let index = 0; index < counter; index++) {
  if(index == 0){
  index++
  }
  message_edit = parseInt(index, 10)
  print_message = message;
  print_message += ' ';
  print_message += message_edit;
  textbox.innerHTML = print_message;
  textbox.dispatchEvent(event);
  setTimeout(wait, 10000);
  document.getElementsByClassName("tvf2evcx oq44ahr5 lb5m6g5c svlsagor p2rjqpw5 epia9gcq")[0].click();
}
function wait() {
}
------------------------------------------------------------------------------------------------------- ignore this  >>>>>

function sleep(ms) {
    return new Promise(resolve => setTimeout(resolve, ms));
}

async function demon() {
    for (let i = 0; i < 5; i++) {
        console.log(`Waiting ${i} seconds...`);
        await sleep(i * 1000);
    }
    console.log('Done');
}

demon();
------------------------------------------------------------------------------------------------------- ignore this  <<<<<<


-------------------------------------------------------------------------------------------------------
Version 1
-------------------------------------------------------------------------------------------------------
function sleep(ms) {
    return new Promise(resolve => setTimeout(resolve, ms));
}

async function demon() {
  var message = prompt("Enter your message", "‎");
  var counter = parseInt(prompt("How many Times ?", 10));
  window.InputEvent = window.Event || window.InputEvent;
  var event = new InputEvent("input", { bubbles: true });
  var textbox = document.getElementsByClassName("_13NKt copyable-text selectable-text")[1];
  for (let index = 0; index < counter; index++) {
    if(index == 0){
    index++
    }
    message_edit = parseInt(index, 10)
    print_message = message;
    print_message += ' ';
    print_message += message_edit;
    textbox.innerHTML = print_message;
    await sleep(10 * 1000);
    textbox.dispatchEvent(event);
    document.getElementsByClassName("tvf2evcx oq44ahr5 lb5m6g5c svlsagor p2rjqpw5 epia9gcq")[0].click();
}
}

demon();



-------------------------------------------------------------------------------------------------------
```
