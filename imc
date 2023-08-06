
const calcular = document.getElementById('calcular')


function imc(){
  const resultado = document.getElementById('resultado')
  const nome = document.getElementById('nome').value
  const altura = document.getElementById('altura').value
  const peso = document.getElementById('peso').value

  if(nome.value !== '' && altura !== '' && peso !== ''){
    
    const valorIMC = (peso / (altura * altura) ).toFixed(1)

    let classificar = ''

    if( valorIMC < 18.5){
       classificar = 'abaixo do peso.'
    } else if ( valorIMC < 25){
      classificar = 'com peso ideal.Parabéns!'
    } else if( valorIMC < 30){
      classificar = 'levemente acima do peso.'
    }else if ( valorIMC < 35){
      classificar = 'com obesidade grau I.'
    }else if ( valorIMC < 40 ){
      classificar = 'com obesidade grau II.'
    }else {
      classificar = 'com obesidade grau III. Cuidado!'
    }
    

    resultado.textContent = `${nome} seu IMC é ${valorIMC} você está ${classificar}`

  }else{
    resultado.textContent = 'Preencha todos os campos!!'
  }
}


calcular.addEventListener('click', imc)
