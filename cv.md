# Mekan Esenjanov
---
### Junior Frontend Developer
#### Contact information:
***Phone:*** +375298699787

__E-mail:__ Mekan.es1997@gmail.com

__Telegram:__ [@Mekan](https://t.me/Mekan997)
===
## About myself:
Something interesting about me.

## Skills:
* HTML, CSS,JS
* React, Redux, Typescript basics
* Rest API basics
* React-Redux Api basics
## Code examples:
Kata: RGB To Hex Conversion
The rgb function is incomplete. Complete it so that passing in RGB decimal values will result in a hexadecimal representation being returned. Valid decimal values for RGB are 0 - 255. Any values that fall out of that range must be rounded to the closest valid value.

Note: Your answer should always be 6 characters long, the shorthand with 3 will not work here.

The following are examples of expected output values:
```
rgb(255, 255, 255) // returns FFFFFF
rgb(255, 255, 300) // returns FFFFFF
rgb(0,0,0) // returns 000000
rgb(148, 0, 211) // returns 9400D3
```
Solution:
 ```
  function rgb(r, g, b){
        let z= [r,g,b];

        let x = []
        for(i=0;i<z.length;i++){
            if(z[i]>255){
                x.push(255)
            } else if(z[i]<0){
                x.push(0)
            } else {
                x.push(z[i])
            }
        }
        let c = []
        let v = ""
        for(j=0;j<x.length;j++){
            let ghgh = Math.floor(x[j]/16)
            c.push(ghgh)
            c.push(x[j] - ghgh*16 )
        }
        for(k=0;k<c.length;k++){
            if(c[k]===10){
                v= v+"A"
            }if(c[k]===11){
                v= v+"B"
            }if(c[k]===12){
                v= v+"C"
            }if(c[k]===13){
                v= v+"D"
            }if(c[k]===14){
                v= v+"E"
            }if(c[k]===15){
                v= v+"F"
            }else if(c[k]<10){
                v=v+c[k]
            }
        }
       return v
    }
   
