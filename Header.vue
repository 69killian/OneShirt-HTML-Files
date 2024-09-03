<script></script>

<template>
<header>
        <div class="header-left-hand">
            <img class="logo" src="images/ONSHIRT NOIR 11.png" alt="OneShirt">
            <input class="recherche" type="text" placeholder="Rechercher">
        </div>
        <div class="header-right-hand">
            <p>Boutique</p>
            <p>Blog</p>
            <p>A propos</p>
            <p>Contact</p>
            <button>Connexion</button>
            <button>Panier 0</button>
        </div>
    </header>
</template>

<style>

header {
    display: flex;
    align-items: center;
    justify-content: space-between;
    background-color: aqua;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    height: 70px;
    padding: 0 20px;
    z-index: 1000;
}

.header-right-hand {
    display: flex;
    align-items: center;
    gap: 20px;
}

.header-left-hand {
    display: flex;
    align-items: center;
    gap: 20px;
    flex-grow: 1; 
}

.recherche {
    border: 1px solid rgb(181, 181, 181);
    padding: 10px;
    width: 100%;
    max-width: 500px; 
    border-radius: 100px;
    color: black;
    transition: width 0.3s ease; 
}

.logo {
    height: 50px; 
    width: auto;
}


@media (max-width: 768px) {
    .recherche {
        max-width: 300px; 
    }

    .logo {
        height: 40px; 
    }
}


@media (max-width: 480px) {
    .recherche {
        max-width: 200px; 
    }

    .logo {
        height: 30px; 
    }

    .header-right-hand {
        gap: 10px; 
    }

    header {
        flex-direction: column; 
        height: auto;
        align-items: flex-start; 
    }

    .header-left-hand, .header-right-hand {
        width: 100%;
    }

    .header-right-hand {
        order: 2; 
        justify-content: flex-start; 
        margin-top: 10px; 
    }

    .header-left-hand {
        order: 1; 
    }
}

</style>