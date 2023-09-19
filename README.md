# Animation_project

 <style>
        .animate{
            width: 400px;
            height: 400px;
            border: 3px solid black;
            margin: auto;
            position: relative;
        }
        .small{
            width: 80px;
            height: 80px;
            border: 3px solid black;
            background-color:red;
            position: absolute;
            top:0px;
            left: 0px;
            /*
            animation-name: small;
            animation-duration: 5s;
            */
            animation: small 5s; 
            animation-delay: 2s;
            animation-iteration-count: 5;
            animation-fill-mode: forwards;
            animation-direction: reverse;
        
        }

        @keyframes small{
               0%{
                top: 0px;
                left: 0px;
                background-color: red;
               }

                40%{
                    top: 0px;
                    left: 316px;
                    background-color: rgb(214, 133, 33);
                }

                50%{
                    top: 316px;
                    left: 316px;
                    background-color: blue;
                }

                75%{
                    top: 316px;
                    left: 0px;
                    background-color: lawngreen;
                }

                100%{
                    top: 0px;
                left: 0px;
                background-color: red;
                }
        }

        .linear{
            width: 600px;
            height: 200px;
            border: 2px solid black;
            margin: auto;
            position: relative;
        }

        .ease{
            width: 90px;
            height: 50px;
            border: 2px solid red;
            background-color: blue;
            margin-top: 75px;
            position: absolute;
            animation-name: ease;
            animation-duration: 5s;
            animation-iteration-count: 2;
            /*
            animation-timing-function: linear;
            */
            /*
                        animation-timing-function: ease;
                        */
                        /*
                animation-timing-function: ease-in;
                */
                /*
                animation-timing-function: ease-out;
                */
                animation-timing-function: ease-in-out;

        }

         @keyframes ease{
            from{
                left: 0px;
            }
            to{
                left: 506px;
            }
         }
     </style>
</head>
<body>
        <div class="animate">
                  <div class="small">
                  </div>
        </div>
         <div class="linear">
                   <div class="ease">
                   </div>
         </div>
</body>
