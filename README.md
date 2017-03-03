# ES6-Filtering-And-Mapping

// jshint esnext: true

const array = [40, 45, 37, 39, 40, 38, 37, 48, 32, 47, 43, 41, 38, 31, 48, 36, 30, 39, 36, 30, 48, 42, 45, 36, 44];

console.log('array', array);

function Below40(value){ return value < 40;
}

const isBelow40 = [40, 45, 37, 39, 40, 38, 37, 48, 32, 47, 43, 41, 38, 31, 48, 36, 30, 39, 36, 30, 48, 42, 45, 36, 44].filter(Below40);

console.log('Values below 40:', isBelow40);

function Above35(value){ return value > 35; }

const isAbove35 = [37, 39, 38, 37, 32, 38, 31, 36, 30, 39, 36, 30, 36].filter(Above35);

console.log('Values above 35 and below 40:', isAbove35);

var numbers = [37, 39, 38, 37, 38, 36, 39, 36, 36];

var roots = numbers.map(function(x){ return x * 2; });

console.log('Values which are greater than 35, less than 40, and then doubled:', roots);

