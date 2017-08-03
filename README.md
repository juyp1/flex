# flex
flex web布局   
flex布局分为旧版本dispaly: box;，过渡版本dispaly: flexbox;，以及现在的标准版本display: flex;

Android
  2.3 开始就支持旧版本 display:-webkit-box;
  4.4 开始支持标准版本 display: flex;

IOS
  6.1 开始支持旧版本 display:-webkit-box;
  7.1 开始支持标准版本 display: flex;

PC
  如果你不需要兼容ie10以下版本，也是可以使用flex.css

flex.css同时能兼容新版本和旧版本，保证了浏览器不支持新版本时，回退到旧版本。   

# Use   
  将dist目录下的css文件引入到你的页面中，根据你的需要引入  
  
  flex.css 使用flex属性匹配  
  
  data-flex.css 使用data-flex属性匹配（React使用）  
  
  
  如果使用了webpack打包，npm安装后，并且配置了ES6编译器的话， 
  flex 属性匹配可以直接使用： 
  
    import 'flex.css';  
    
  data-flex 属性匹配可以直接使用(react使用)  
  
    import 'flex.css/dist/data-flex.css'; 
  
 
# 常用的属性配置   
dir：主轴方向  
    top：从上到下  
    right：从右到左  
    bottom：从下到上  
    left：从左到右（默认）  
     
 main：主轴对齐方式  
    right：从右到左   
    left：从左到右（默认）  
    justify：两端对齐  
    center：居中对齐  
    
cross：交叉轴对齐方式  
    top：从上到下（默认） 
    bottom：从上到下  
    baseline：基线对齐  
    center：居中对齐  
    stretch：高度并排铺满  
 
box：子元素设置  
    mean：子元素平分空间  
    first：第一个子元素不要多余空间，其他子元素平分多余空间  
    last：最后一个子元素不要多余空间，其他子元素平分多余空间  
    justify：两端第一个元素不要多余空间，其他子元素平分多余空间  
    
 
 # flex-box属性说明
 取值范围(0-10)，单独设置子元素多余空间的如何分配，设置为0，则子元素不占用多余的多余空间  
多余空间分配 = 当前flex-box值/子元素的flex-box值相加之和
