# Features : 

### Menu Mobile : 

Para la construcion del Menu Mobile,se creo un menu hamburguesa haciendo el cual al mamomento de recibir el evento click se activa un checked , que despliega el menubar.

#### Código : :

HTML :
```html
    <nav class="nav  fadeInDown">
            <a href="">
                <img loading="lazy"  src="assets/images/logo.svg" alt="logo blue dot">
            </a>
                <input id="burger" type="checkbox" />
                <label for="burger"> 
                    <span></span>
                    <span></span>
                    <span></span>
                </label>
                </div>
                <ul class="menubar fadeInDownMenu">
                    <li><a href="#episodios"> Episodios</a></li>
                    <li><a href="#nosotros">Nosotros</a></li>
                    <li><a href="#invitadas">Entrevistas</a></li>
                    <li><a href="#temas">Tópicos</a></li>
                </ul>
        </nav>

```
CSS :: 

```CSS
        input {
  display: none;
}

label {
  position: fixed;
  top: 10px;
  right: 16px;
  height: 20px;
  width: 20px;
  z-index: 5;
}

input + label span {
  position: absolute;
  width: 100%;
  height: 2px;
  top: 50%;
  margin-top: -1px;
  left: 0;
  display: block;
  background: #020304;
  -webkit-transition: 0.5s;
  transition: 0.5s;
}

input + label span:first-child {
  top: 3px;
}

body input + label span:last-child {
  top: 16px;
}

label:hover {
  cursor: pointer;
}

input:checked + label span {
  opacity: 0;
  top: 50%;
}

input:checked + label span:first-child {
  opacity: 1;
  -webkit-transform: rotate(405deg);
          transform: rotate(405deg);
}

input:checked + label span:last-child {
  opacity: 1;
  -webkit-transform: rotate(-405deg) translate(4.5px, -4.5px);
          transform: rotate(-405deg) translate(4.5px, -4.5px);
}

```


```CSS
header .nav .menubar {
  display: none;
}

header .nav input:checked ~ .menubar {
  position: absolute;
  left: 0;
  top: 100%;
  display: block;
  background: #0000EC;
  width: 100vw;
  height: 40vh;
  list-style: none;
  display: block;
}

header .nav input:checked ~ .menubar li {
  padding-top: 16px;
  margin-left: 16px;
  margin-bottom: 24px;
}

header .nav input:checked ~ .menubar a {
  color: #ffffff;
  text-decoration: none;
  font-size: 16px;
  text-transform: uppercase;
  margin-bottom: 24px;
}
```
