# -
import Foundation
var a=[1,4,3,5,3,6,7,8,9,0]
var i=0
var j=0
var t=0
for i in 0...9
{
    print(a[i])
}

for i in 0..<a.count - 1{
    for j in 0..<a.count - i - 1{
        if a[j] < a[j+1]{
           t = a[j]
            a[j] = a[j+1]
            a[j+1] = t
        }
    }
}
print()
for i in 0...9
{
    print(a[i])
}
