# FontAwesome5WithApacheFlex
Just a simple demo that shows how to use FontAwesome5 with Apache Flex

![alt text](https://github.com/olafkrueger/FontAwesome5WithApacheFlex/blob/master/OutputDemoApplication.PNG "Demo")



Use FontAwesome5 within your Apache Flex application in four steps. It's pretty straightforward:

#### 1. Download [FontAwesome5](https://use.fontawesome.com/releases/v5.0.6/fontawesome-free-5.0.6.zip)

#### 2. Grap the *.otf files from the "use-on-desktop" directory and paste it into your Flex project

#### 3. Apply the fonts by some style declaration

```
<fx:Style>
		@namespace s "library://ns.adobe.com/flex/spark";
		@namespace mx "library://ns.adobe.com/flex/mx";
		
		
		@font-face { 
			src: url("fonts/FontAwesome5FreeRegular400.otf"); 
			fontFamily: FontAwesome5Regular;
			embedAsCFF: true;
		}
		
		@font-face { 
			src: url("fonts/FontAwesome5FreeSolid900.otf"); 
			fontFamily: FontAwesome5Solid;
			embedAsCFF: true;
		}
		
		@font-face { 
			src: url("fonts/FontAwesome5BrandsRegular400.otf"); 
			fontFamily: FontAwesome5Brands;
			embedAsCFF: true;
		}	
</fx:Style>
```
Spaces and hyphens are removed from otf file names here.


#### 4. Use it with e.g. the spark Label component
```
<s:Label text="\uf058" fontFamily="FontAwesome5Regular" fontSize="100" color="#000000" />
```
You find a list of all icons in the [CheatSheet](https://fontawesome.com/cheatsheet).
