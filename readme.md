1) First error message I got main.js:43 Uncaught TypeError: Cannot read properties of null (reading 'length')
        Fix: to fix this error i used a condition on line number 40. when I parse in JSON localStorage.getItem('essues'). some essues are null. then I use condition becouse if essues are null then it will be return.


2) Second error: when I click the close button I got this error Uncaught ReferenceError: setStatusClosed is not defined.
        Fix: here setStatusClosed() is called on close button but it is not define other place. there is a function for close button but it is not call on close button. i replace closeIssue() insted of setStatusClosed.

3) Third error: the other error is Uncaught TypeError: Cannot set properties of undefined (setting 'status')
    at closeIssue (main.js:27)
        Fix: there is a compare operator. one is essue.id which is a string and other is id which number. we have to convert essue.id in number.

4) Forth error: the error is undefined on line number 34.
        Fix: it is forEatch method error. here no parameter on forEatch. 

Bonux: when i click delet button it work properly but the page have to reload manualy. thats why i add a function location.reload() on close button.