*{
    margin: 0;
    padding: 0;
}
html{
    font-size: 100%;
    scroll-behavior: smooth;
}
body{
    overflow-x: hidden;
    font-family: Arial, Helvetica, sans-serif;

}
/* hero section */
/* #hero{ */
    /* position: relative;
    width: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
} */
#hero{
    position: relative;
    width:100vw ;
    height: 100vh;
    display: flex;
    justify-content:center ;
    align-items: center;
    text-align: center;
}
 #hero::before{
    content:"" ;
    position: absolute;
    top: 0;
    width: 100%;
    height: 100%;
    background-image: url(doordash-restaurant-zoom-backgrounds.webp);
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center center;
    background-attachment: fixed;
    filter:brightness(50%)

}
#hero-content{
    position: absolute;
    
}
#hero-content h1{
    
    color: #fff;
    font-size: 2.8rem;
    text-shadow: 2px 2px 2px #000;
    
    
}

#hero-content h2{
    
    color:gold;
    font-size: 2rem;
    font-family: cursive;
    margin-top: 1rem;
    margin-bottom: 4rem;
    text-shadow: 2px 2px 2px #000;
    
}
#hero-content a{
    color: #fff;
    padding: 3px 20px 3px 20px;
    border: 1px solid orange;
    background: rgb(0, 0 ,0, 0.6);
    font-size: 1.5rem;
    text-decoration: none;
border-radius: 25px;
}
#hero-content a:hover{
    background: goldenrod
}
/* ---------------- */
/* header section */
#header{
    position: fixed;
    top: 0;
    width: 100vw;
    height: 70px;
    line-height: 70px;
}

#navbar{
    display: flex;
    justify-content: space-around;
    background: rgb(0, 0 ,0, 0.5);
}
#header h1{
    color: orange;
    font-size: 1.8rem;
    text-shadow: 2px 2px 2px #000;
    font-family: cursive;
    
}
#navbar ul{
    display: flex;

}



#navbar ul li{
    list-style: none;
    padding: 3px 15px 3px 15px;
}
#navbar ul li:hover,#phone a:hover,#mobile-menu ul li:hover{
    background: navy;
    cursor: pointer;
}
#navbar ul li a{
    color: #fff;
    text-decoration: none;
    font-size: 1.1rem;
}
#phone a{
    color: #fff;
    text-decoration: none;
    font-size: 1.1rem;
    padding: 3px 15px 3px 15px ;
    border: 1px solid orange;

}
#mobile-menu{
    display: none;
    height: 40px;
    line-height: 40px;
    background-color: magenta;
}
#mobile-menu ul{
    display: flex;
    justify-content: center;
}
#mobile-menu ul li{
    list-style: none;
    padding: 0.5px 0.5px;
}
#mobile-menu ul li a{
    text-decoration: none;
    color: #fff;
}


@media screen and(max-width:768px){
    #mobile-menu{
        display: block;
    }
    #navbar ul{
        display: none;
    }
    html{
        font-size: 70%;
    }
    #menu-row,#about-row,#contact-row{
        flex-wrap: wrap;
        padding: 0 10px 0 10px;
    }
    #about-img{
        width: 220;
        height: 220;
    }
}
@media screen and(max-width:768px){
    
}


/* menu section */

#menu{
    padding: 25px 0px 25px 0px;
}
    #section{
        padding: 25px 0px 25px 0px;
        text-align: center;
        font-size: 2rem;
        font-family: verdana;

    }
    #menu-row{
        display: flex;
        padding: 0px 100px 0px 100px ;
    }
    #menu-col{
        box-shadow: 2px 2px 2px #bbb;
        background-color: #fff;
        margin: 10px;
        padding: 10px;
        flex: 1;
    }
#menu-col h2{
    background-color:red;
    color: #fff;
    text-align: center;
    padding: 5px;
    font-family: cursive;
}
#image{
    width: 150px;
    height: 150px;
    border-radius: 50%;
    padding: 5px;
    border: 2px solid orange;
}
#image img{
    width: 100%;
    height: 100%;
    border-radius: 50%;
    object-fit: cover;
}
.box{
    display: flex;
    flex-direction: column;
    align-items: center;
    text-align: center;
    margin: 5px;

}
/* chef section begin */

#chef{
    padding: 25px 0 25px 0;

}
#chef-row{
    display: flex;
    justify-content: center;
}
.chef-col{
    text-align: center;
    padding: 10px;
    margin: 5px;
}
#img{
    width: 200px;
    height: 250px;
    margin: auto;
}
#img img{
    width: 100%;
    height: 100%;
    object-fit: cover;
}
/* chef section :end */
   

/* about section begin*/

#about{
    padding: 25px 0 25px 0;
}
#about-row{
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    padding: 0 100px 0 100px;

}
.about-col{
    flex: 1;
}
#about-img img{
    position: center;
    padding-top: 10%;
}


.about-col h1{
    text-align: center;
    font-family: cursive;
}
   .about-col p{
    text-align: justify;
    font-weight: bold;

   }



/* about section :end */

/* contact section begin */

#contact{
    padding: 25px 0 25px 0;
}
#contact-row{
    display: flex;
    justify-content: center;
    align-items: center;
    padding: 0 100px 0 100px;
    flex-wrap: wrap;
}
.contact-col{
    display: flex;
    flex-direction: column;
    align-items: center;
    flex: 1;
}
.contact-col p,h3{
    font-weight: bold;
    color: #292929;
    margin: 10px;
}
.contact-col p a{
    text-decoration: none;
    color: #292929;
}
#social a{
    color: magenta;
    margin: 3px;
}
.contact-col form{
    display: flex;
    flex-direction: column;
    background-color: magenta;
    width: 70%;
    padding: 20px 40px 20px 20px;
}
.contact-col form h2{
    text-align: center;
    font-family: cursive;
}
.contact-col form input{
    width: 100%;
    height: 17pt;
    padding: 5px;
    margin: 5px;
}
.contact-col form textarea{
    width: 100%;
    padding: 5px;
    margin: 5px;
}
.contact-col form button{
    margin: auto;
    padding: 10px;
    color: #fff;
    background-color: orange;
    border: 1px solid orange;
}


/* contact section :end */
/* footer section */
#footer{
    background-color: #292929;
    padding: 20px;
    position: relative;
}
#footer h5{
    text-align: center;
    color: orange;
}
#footer h5 a{
    color: #fff;
    text-decoration: none;
}
#top{
    position: absolute;
    bottom: 12px;
    right: 12px;
}
#top a{
    color: #fff;
    font-size: 1.2rem;
}




/* footer section :end */

# neha
