var intToRoman = function(num) {
  let rNum = '';
    let numArr = num.toString().split('');
  
    for (let i = 0; i < numArr.length; i++) { 
      let backToNum = parseInt(numArr[i]);
      if (numArr.length - i === 4) { // 3999 --> 4 - 0 = 4
        if (backToNum < 4) {
          let i = 0;
          while(i < backToNum){
            rNum += 'M';
            i++;
          }
        }
      } 
      if (numArr.length - i === 3) { // 999 --> 4 - 1 = 3
        if (backToNum === 4) {
          rNum += 'CD';
        } else if (backToNum === 5) {
          rNum += 'D';
        } else if (backToNum < 4) {
          let i = 0;
          while (i < backToNum) {
            rNum += 'C';
            i++;
          }
        } else if (backToNum === 9) {
          rNum += 'CM';
        } else if (backToNum > 5) {
          let j = 5;
          rNum += 'D'
          while( j < backToNum) {
            rNum += 'C';
            j++;
          }
        }
      }
      if (numArr.length - i === 2) { // 99 --> 4 - 2 = 2
        if (backToNum === 4) {
          rNum += 'XL';
        } else if (backToNum === 5) {
          rNum += 'L';
        } else if (backToNum < 4) {
          let i = 0;
          while (i < backToNum) {
            rNum += 'X';
            i ++;
          }
        } else if (backToNum === 9) {
          rNum += 'XC';
        } else if (backToNum > 5) {
          let j = 5;
          rNum += 'L';
          while (j < backToNum) {
            rNum += 'X';
            j++;
          }
        }
      }
      if (numArr.length - i === 1){ // 9 --> 4 - 3 = 1;
        if (backToNum === 4) {
          rNum += 'IV';
        } else if (backToNum === 5) {
          rNum += 'V';
        } else if (backToNum < 4) {
          let i = 0;
          while (i < backToNum) {
            rNum += 'I';
            i++;
          }
        } else if (backToNum === 9) {
          rNum += 'IX';
        } else if (backToNum > 5) {
          let j = 5;
          rNum += 'V';
          while (j < backToNum) {
            rNum += 'I';
            j++;
          }
        }
      } 
    }
    return rNum;
  };
