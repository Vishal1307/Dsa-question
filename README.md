# Dsa-question
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
