    .systeme-solaire {
        position: relative;
        width: 600px;
        height: 600px;
        margin: 50px auto;
    }

    .soleil {
        position: absolute;
        top: 50%;
        left: 50%;
        width: 80px;
        height: 80px;
        background-color: yellow;
        border-radius: 50%;
        transform: translate(-50%, -50%);
        box-shadow: 0 0 50px yellow;
    }

    .orbite {
        position: absolute;
        top: 50%;
        left: 50%;
        border: 1px dashed rgba(255, 255, 255, 0.3);
        border-radius: 50%;
        transform: translate(-50%, -50%);
    }

    .planete {
        position: absolute;
        width: 20px;
        height: 20px;
        background-color: lightblue;
        border-radius: 50%;
    }

    /* Planètes et leurs orbites */
    .orbite-mercure { width: 100px; height: 100px; }
    .mercure { background-color: gray; animation: orbit 3s linear infinite; }

    .orbite-venus { width: 150px; height: 150px; }
    .venus { background-color: orange; animation: orbit 5s linear infinite; }

    .orbite-terre { width: 200px; height: 200px; }
    .terre { background-color: blue; animation: orbit 8s linear infinite; }

    .orbite-mars { width: 250px; height: 250px; }
    .mars { background-color: red; animation: orbit 10s linear infinite; }

    @keyframes orbit {
        from { transform: rotate(0deg) translateX(50px) rotate(0deg); }
        to { transform: rotate(360deg) translateX(50px) rotate(-360deg); }
    }

    /* Ajustement de la position des planètes sur leurs orbites */
    .mercure { top: 50%; left: 50%; transform: translate(-50%, -50%); }
    .venus { top: 50%; left: 50%; transform: translate(-50%, -50%); }
    .terre { top: 50%; left: 50%; transform: translate(-50%, -50%); }
    .mars { top: 50%; left: 50%; transform: translate(-50%, -50%); }
</style>
    
    <div class="orbite orbite-mercure">
        <div class="planete mercure"></div>
    </div>
    <div class="orbite orbite-venus">
        <div class="planete venus"></div>
    </div>
    <div class="orbite orbite-terre">
        <div class="planete terre"></div>
    </div>
    <div class="orbite orbite-mars">
        <div class="planete mars"></div>
    </div>
</div>
