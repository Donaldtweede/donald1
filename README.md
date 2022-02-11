# donald1
num = 54;
const isFib = query => {
  if(query === 0 || query === 1){
    return true;
  }
  let prev = 1;
  let count = 2;
  let temp = 0;
  while(count <=query){
    if(prev + count === query){
      return true;
    };
    temp = prev;
    prev = count;
    count += temp;
  };
  return false;
};
console.log(isFib(num));0
