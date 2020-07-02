# Animaciones : : 

Se tomaron animaciones de  <a href="https://animate.style/">Animate Syle</a>.

 - fadeInDown
        
    ```css
            .fadeInDown{
                    animation-duration: 1s;
                    animation-fill-mode: both;
                    animation-name: fadeInDown;
                    }
    ```
    ```css
        @keyframes fadeInDown {
        from{
            opacity: 0;
            transform: translate3d(0,-100%,0);
        }
            to{
                opacity: 1;
                transform: translate3d(0,0,0) ;
            }
    }
    ```
- fadeInDown : 

```css
        .fadeInDownMenu{
            animation-duration: .1s;
            animation-fill-mode: both;
            animation-name: fadeInDownMenu;
            }
```

```css
        @keyframes fadeInDownMenu {
            from{
                opacity: 0;
                transform: translate3d(0,-100%,0);
            }
                to{
                    opacity: 1;
                    transform: translate3d(0,0,0) ;
                }
            }
```

- slideInLeft

```css
                .slideInLeft{
                animation-duration: 1s;
                animation-fill-mode: both;
                animation-name: slideInLeft;
                }

```

```css
               
@keyframes slideInLeft {
  from {
    transform: translate3d(-100%, 0, 0);
    visibility: visible;
  }

  to {
    transform: translate3d(0, 0, 0);
  }
}

```