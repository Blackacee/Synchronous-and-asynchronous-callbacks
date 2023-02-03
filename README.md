# Synchronous-and-asynchronous-callbacks

/**
 * @arg {Function} then continuation callback
 */
function doSomething(then) {
 console.log('Doing something');
 then();
}
// Do something, then execute callback to log 'done'
doSomething(function () {
 console.log('Done');
});
console.log('Doing something else');
