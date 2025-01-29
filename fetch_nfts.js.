const userHandle = "cNieves"; // Tu usuario en Objkt.com
const apiUrl = `https://api.objkt.com/v3/users/${userHandle}/creations`;

// Función para obtener la cantidad de NFTs creados
async function fetchNFTs() {
    try {
        const response = await fetch(apiUrl);
        
        if (!response.ok) {
            throw new Error(`Error ${response.status}: No se pudo obtener la información`);
        }

        const data = await response.json();
        console.log(`Número de NFTs creados por ${userHandle}: ${data.length}`);
    } catch (error) {
        console.error("Error:", error.message);
    }
}

// Ejecutar la función
fetchNFTs();
