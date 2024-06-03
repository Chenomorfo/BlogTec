<nav>
    <ul>
        <li>
            <details>
                <summary>Que es?</summary>
                <ul>
                    <li>Introduccion</li>
                    <li>Donde descargar</li>
                    <li>Guia rapida</li>
                    <li>El creador de GIT</li>
                    <li>Utilidad</li>
                    <li>Test</li>
                </ul>
            </details>
        </li>
        <li>
            <details>
                <summary>CLI</summary>
                <ul>
                    <li>Resumen de</li>
                    <li>Comandos basicos</li>
                    <li>Comandos avanzados</li>
                    <li>Commits</li>
                    <li>Logs</li>
                    <li>Branches</li>
                    <li>Test</li>
                </ul>
            </details>
        </li>
        <li>wasap</li>
    </ul>
</nav>

<style>
    nav {
        background-color: #575555;
        color: white;
        text-transform: uppercase;
        padding-left: 12px;
        padding-top: 8px;
        padding-bottom: 20px;
        height: 100%;
        width: 250px;
    }
    nav ul li,
    details > summary {
        font-size: 1.5rem;
    }
    ul {
        margin-left: 26px;
    }
    ul li {
        position: relative;
        list-style: none;
        user-select: none;
        padding: 2px 0;
    }
    li::before,
    li::after {
        content: "";
        position: absolute;
        left: -22px;
        background-color: white;
    }
    li::before {
        height: 2px;
        width: 16px;
        top: 22px;
    }
    li::after {
        height: 36px;
        width: 2px;
        top: -14px;
    }

    li:has(details)::after {
        height: 100%;
        top: 12px;
    }
    li:has(details):last-child::after {
        content: none;
    }
    details {
        margin: 0 auto;
        max-height: 36px;
        transition: max-height 1.2s linear;
    }
    summary {
        display: block;
        position: relative;
        cursor: pointer;
        transition: all 0.3s ease;
        padding: 3px 5px;
    }
    summary:hover {
        margin-left: 10px;
    }
    details[open] {
        max-height: 1000px;
    }
    details[open] > summary {
        background-color: white;
        color: black;
        border-radius: 12px;
        margin-right: 5px;
        margin-left: 10px;
    }

    details ul {
        padding-top: 8px;
        margin-left: 12px;
    }

    details ul li {
        padding: 2px 0;
        font-size: 1rem;
        transition: all .3s ease-in-out;
        cursor: pointer;
    }

    details ul li:hover{
        padding-left: 5px;
    }

    

    details ul li::before {
        top: 14px;
        width: 18px;
    }
    details ul li::after {
        height: 30px;
    }

    details ul li:first-of-type::after {
        height: 38px;
        top: -20px;
    }
</style>
