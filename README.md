# Dsa-question
**#binary upper bound**
function isTrue(n,k,ary){
    var low=1
    var high=n
    var ans=-1
    while(low<=high){
        var mid=Math.floor(low+(high-low)/2)
        if(ary[mid]<=k){
            
            low=mid+1
            
        }
        
        else{
            ans=mid
            high=mid-1
        }
    }
    return ans
}


****lower bound
_function isTrue(n,k,ary){
    var low=0
    var high=n-1
    var ans=-1
    while(low<=high){
        var mid=Math.floor(low+(high-low)/2)
        if(ary[mid]==k){
            ans=mid
            high=mid-1_
            
        }
        else if(ary[mid]>k){
            high=mid-1
        }
        else{
            low=mid+1
        }
    }
    return ans
}
**binary serch**

var arry=[1,2,3,4,5,6]
var k=4
function binary(arry,k){
  var low=0
  var high=arry.length-1
  while(low<=high){
    
    var mid=Math.floor((low+high)/2)
    if(arry[mid]==k){
      return mid
    }
    else if(arry[mid]<k){
      low=mid+1
    }
    else{
      high=mid-1
    }
  }
  
}
console.log(binary(arry,k))





