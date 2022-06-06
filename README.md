
#Sensores de Movimento Nativos de Reação
#Começando
$ npm install react-native-motion-sensors --save

#Principalmente instalação automática
$ react-native link react-native-motion-sensors

#Instalação manual
#iOS
No XCode, no navegador do projeto, clique com o botão direito do mouse Libraries➜Add Files to [your project's name]
Vá para node_modules➜ react-native-motion-sensorse adicioneRNMotionSensors.xcodeproj
No XCode, no navegador do projeto, selecione seu projeto. Adicione libRNMotionSensors.aao seu projeto Build Phases➜Link Binary With Libraries
Execute seu projeto ( Cmd+R)<

#Android
Abraandroid/app/src/main/java/[...]/MainActivity.java
Adicionar import com.reactlibrary.RNMotionSensorsPackage;às importações na parte superior do arquivo
Adicionar new RNMotionSensorsPackage()à lista retornada pelo getPackages()método
Anexe as seguintes linhas a android/settings.gradle:
include ':react-native-motion-sensors'
project(':react-native-motion-sensors').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-motion-sensors/android')
Insira as seguintes linhas dentro do bloco de dependências em android/app/build.gradle:
  compile project(':react-native-motion-sensors')
janelas
Leia-o! :D

#No Visual Studio, adicione a pasta RNMotionSensors.slnin à sua solução, referência de seu aplicativo.node_modules/react-native-motion-sensors/windows/RNMotionSensors.sln
Abra seu MainPage.csaplicativo
Adicione using Com.Reactlibrary.RNMotionSensors;aos usos no topo do arquivo
Adicione new RNMotionSensorsPackage()ao List<IReactPackage>retornado pelo Packagesmétodo
Uso
import RNMotionSensors from 'react-native-motion-sensors';

// TODO: What to do with the module?
RNMotionSensors;
