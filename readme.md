### Bug?

When I run a code an arbitary code like `bg-[url('...')]` it creates a new folder called static with some wierd subfolders. Even if the requested file is in the assets folder!

Problem: I need to define a path while using the arbitary value like `public/assets/img.png`. However if I create a simple css line like `background: url('/assets/img.png')` it works. However this will only work if this line is put in the browser because doing it in the file itself will create the weird folder structure. Not using `public/` gives out an error. Why would the img be put in the `static` folder and not the actual `assets` folder?

### Where is the code reproduction?

Just visit the `bug` folder and follow these steps

1. run `npm ci`
2. run `npm run build`
3. go in the `build` folder and see the monster folder called `static`
