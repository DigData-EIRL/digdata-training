# Docker

Docker es un proyecto de código abierto para automatizar la implementación de aplicaciones como contenedores portátiles y autosuficientes que se pueden ejecutar en la nube o localmente. Docker es también una empresa que promueve e impulsa esta tecnología, en colaboración con proveedores de la nube, Linux y Windows, incluido Microsoft.

En esta práctica se implementará Docker en el proyecto de la práctica anterior, por lo que necesitas completar las prácticas anteriores antes de seguir con esta.

**¿Para que se usa Docker?**

<!-- Agregar investigacion -->

**¿Qué es una imagen en Docker?**

<!-- Agregar investigacion -->

**¿Qué es un contenedor en Docker?**

<!-- Agregar investigacion -->

## Instalación de Docker

1. Ir a la página oficial de Docker: [https://hub.docker.com/editions/community/docker-ce-desktop-windows/](https://hub.docker.com/editions/community/docker-ce-desktop-windows/)
2. Descargar el archivo ejecutable.
3. Ejecuta el archivo descargado.
4. Para comprobar la instalación escribe "_docker --version_" \*\*en el CMD o línea de comando. Si hiciste todo bien debería salir algo como esto:

![https://lh4.googleusercontent.com/pZPKdJ_UUAM3X4UYJSYInQiUmmhXsvakLEQvWZq6HJtit_6zkqc4iB0KX07_udqSvruNOr_tlGiMovY1_ix-nsvC5HLXV6ztZ-_k23_dK8OvhZWnLr6ZhgZLIXe2qiHMN2w67t4l](https://lh4.googleusercontent.com/pZPKdJ_UUAM3X4UYJSYInQiUmmhXsvakLEQvWZq6HJtit_6zkqc4iB0KX07_udqSvruNOr_tlGiMovY1_ix-nsvC5HLXV6ztZ-_k23_dK8OvhZWnLr6ZhgZLIXe2qiHMN2w67t4l)

## Crear contenedor de la aplicación con React

1. Abre tu aplicación de React en Visual Studio Code.

![https://lh5.googleusercontent.com/-pDoSjQj4CLDIydEb_5_nl-cOIO4-9JQsx7lsRg0o6go4zks0f9iBR-_XRChtinf42nlHRn85SubDAaTLkoCaIZGJy2dPUxMgFLPd32x37ah1SZPACuz4iJWUQ_cGLwwrYn1BBhI](https://lh5.googleusercontent.com/-pDoSjQj4CLDIydEb_5_nl-cOIO4-9JQsx7lsRg0o6go4zks0f9iBR-_XRChtinf42nlHRn85SubDAaTLkoCaIZGJy2dPUxMgFLPd32x37ah1SZPACuz4iJWUQ_cGLwwrYn1BBhI)

2. Abre el terminal de Visual Studio con "_Ctrl + J_". (_este atajo puede variar según el sistema operativo)_

![https://lh4.googleusercontent.com/5sKbrjctwTSssghd2mQls679CNJ-ITjoX7zYB-UiBXfU49Z1r2M8ZBpKVmJXhbOXP8ixZ6_iSTjUIFo_NxxG9oEafhcWxRvrNhRmVJhqmXrmfJfsCjMeJPyNzrU13soCNzy9yknF](https://lh4.googleusercontent.com/5sKbrjctwTSssghd2mQls679CNJ-ITjoX7zYB-UiBXfU49Z1r2M8ZBpKVmJXhbOXP8ixZ6_iSTjUIFo_NxxG9oEafhcWxRvrNhRmVJhqmXrmfJfsCjMeJPyNzrU13soCNzy9yknF)

3. Escribe "_npm run start_" en el terminal para comprobar que todo está funcionando correctamente.

![https://lh5.googleusercontent.com/3BUW3PELPUfznZilraxZvy4RgxL5zK8ZcoeWd31tx7T7OQWGavwsYpFL1z5CH1DhdbhWgNHePx17KwnDQMK1uJkcN2bx2lDTwK7U9dRWewQ19gpv0Da6llY3e0-RVHni5AHjz6mw](https://lh5.googleusercontent.com/3BUW3PELPUfznZilraxZvy4RgxL5zK8ZcoeWd31tx7T7OQWGavwsYpFL1z5CH1DhdbhWgNHePx17KwnDQMK1uJkcN2bx2lDTwK7U9dRWewQ19gpv0Da6llY3e0-RVHni5AHjz6mw)

4. Si se abre la app en tu navegador quiere decir que vas bien.

![https://lh4.googleusercontent.com/ff7O1dSMx8oWmB0upsM9j3yFSSz7Tbd_xHOj3Kqmudoxy3BttHTk1ghND3NXLHfZ4uFRx6iTI5tSqTl4ARrydxxSQ5e1afYLoEw09LOM50nQvPcMDn3oeBcebUCB_wooQbVhK158](https://lh4.googleusercontent.com/ff7O1dSMx8oWmB0upsM9j3yFSSz7Tbd_xHOj3Kqmudoxy3BttHTk1ghND3NXLHfZ4uFRx6iTI5tSqTl4ARrydxxSQ5e1afYLoEw09LOM50nQvPcMDn3oeBcebUCB_wooQbVhK158)

5. Dentro del proyecto, junto al archivo "_package.json_" crea un nuevo archivo llamado "_Dockerfile_".

![https://lh3.googleusercontent.com/RPAosRsWUdhJQ0dMe1pe8r4xq1ZB2XLWCp8zBgliMVTFlcHHG4-T85brht3yk6DfgmFMa0wucQeIM-dg6gnCdy2CJxfMgvY5e5-egg6_pwy4TeLG4XREzXh2YsLex16qlXTL-D7D](https://lh3.googleusercontent.com/RPAosRsWUdhJQ0dMe1pe8r4xq1ZB2XLWCp8zBgliMVTFlcHHG4-T85brht3yk6DfgmFMa0wucQeIM-dg6gnCdy2CJxfMgvY5e5-egg6_pwy4TeLG4XREzXh2YsLex16qlXTL-D7D)

**\*NOTA:** Verifique que el archivo Dockerfile no tenga una extensión de archivo como .txt. Algunos editores pueden agregar esta extensión de archivo automáticamente y esto generaría un error.\*

6. Regresa al terminal de Visual Studio y presiona "_Ctrl + C_" para finalizar la ejecución de la app.

![https://lh4.googleusercontent.com/RgNFkd_MYZLrVdCrNuz9Z7ukAZbOslo8khecyUDOGCLGCq-kMiaXIfrLdvnh8O3w-l4NUNfBOROk-SzX00-7QNcuSkf8pNmbND09bRlbZZF-ttTiyfNwu3iM2wGFvShR-8IqymH3](https://lh4.googleusercontent.com/RgNFkd_MYZLrVdCrNuz9Z7ukAZbOslo8khecyUDOGCLGCq-kMiaXIfrLdvnh8O3w-l4NUNfBOROk-SzX00-7QNcuSkf8pNmbND09bRlbZZF-ttTiyfNwu3iM2wGFvShR-8IqymH3)

7. Escribe "_node --version_" en el terminal para ver la versión de Node que estás usando.

![https://lh3.googleusercontent.com/7l6TzBX52f-8UPQF_N9kzuoBm1VOXXGL_yljqQNTVzQFi4sI7-rzgvzF-0sJZ2tsp8mXFKkNiY6sZGh2xORy-OuOxibw71J951Cd75dR5MC2hXp6ubfv53WbL5Kw0ni1w4W2KzVj](https://lh3.googleusercontent.com/7l6TzBX52f-8UPQF_N9kzuoBm1VOXXGL_yljqQNTVzQFi4sI7-rzgvzF-0sJZ2tsp8mXFKkNiY6sZGh2xORy-OuOxibw71J951Cd75dR5MC2hXp6ubfv53WbL5Kw0ni1w4W2KzVj)

**\*NOTA:** yo estoy usando la versión 14.18.1 (en tu caso este número puede ser diferente).\*

8. Dentro del archivo "_Dockerfile_" coloca lo siguiente:

![https://lh5.googleusercontent.com/DXR9CdQ2HP5jAfu-FqC9HpOxTThVa3fGGcxsjPYYLjUIaYxlSqYO3U56gcc9FOtp6u2Xs3R0dgeMrPQv3NkBlSHC6vgVCoiFsLq9mvLZKPr78fhMrvGVwT70TNpm5emyTQiSqRS8](https://lh5.googleusercontent.com/DXR9CdQ2HP5jAfu-FqC9HpOxTThVa3fGGcxsjPYYLjUIaYxlSqYO3U56gcc9FOtp6u2Xs3R0dgeMrPQv3NkBlSHC6vgVCoiFsLq9mvLZKPr78fhMrvGVwT70TNpm5emyTQiSqRS8)

**\*Nota:** fijate en texto resaltado en la primera línea, ahí debes colocar el número que te salió al escribir* "*node --version*". *Es muy importante que hagas eso para evitar posibles errores.\*

9. Guarda los cambios del archivo "_Dockerfile_" y vuelve al terminal. Dentro del terminal ejecuta "_docker build -t my-app ."_

![https://lh3.googleusercontent.com/WwAwBd_I_R1TsnluJjCDQ00vU2o3qmxHaBRLG69YWg3Ds-59ZuQ8PSSrQ0j0QZrpSqqQ5mIbAD2CXA-9O4oTqY8Olb5QnfpoeuHFqnJxOo7CHsvfqoEqsfC9vGoAAK7mDOfetXZH](https://lh3.googleusercontent.com/WwAwBd_I_R1TsnluJjCDQ00vU2o3qmxHaBRLG69YWg3Ds-59ZuQ8PSSrQ0j0QZrpSqqQ5mIbAD2CXA-9O4oTqY8Olb5QnfpoeuHFqnJxOo7CHsvfqoEqsfC9vGoAAK7mDOfetXZH)

10. Después de esperar unos minutos, debería salirte lo siguiente: (si te sale así vas bien)

![https://lh3.googleusercontent.com/0CUPb7uZ5NY3eZMBi3eYNVEjgBpwF7v87xUDiiXgteYGxx8hePXMxOey9ABeP7bHXpkgq0leHt3gmue9PZg1c8YRtLMCN4OR6mjIq0x6vpjXRYEGYnV1LiW9ZcRnr1ImThGfrJGW](https://lh3.googleusercontent.com/0CUPb7uZ5NY3eZMBi3eYNVEjgBpwF7v87xUDiiXgteYGxx8hePXMxOey9ABeP7bHXpkgq0leHt3gmue9PZg1c8YRtLMCN4OR6mjIq0x6vpjXRYEGYnV1LiW9ZcRnr1ImThGfrJGW)

## Iniciar el contenedor de la aplicación en React

Ahora que tienes el contenedor, ejecutemos la aplicación. Para hacerlo, usaremos el comando "_docker run_".

1. Dentro del terminal ejecuta "d*ocker run -dp 3000:3000 my-app*"

![https://lh3.googleusercontent.com/hW9tSuT4_JynyvdopWqX8oieim2FNz7JkUnEjd6a9JCot020Tf_XdLf0GSuQqf2d1U_J-BASP-OUO_sOBWpI8s95hPfNeQycdWi9E4de2OOb5rv1kHQnS7279lCoyUyoDFIK2fEj](https://lh3.googleusercontent.com/hW9tSuT4_JynyvdopWqX8oieim2FNz7JkUnEjd6a9JCot020Tf_XdLf0GSuQqf2d1U_J-BASP-OUO_sOBWpI8s95hPfNeQycdWi9E4de2OOb5rv1kHQnS7279lCoyUyoDFIK2fEj)

2. Abre el navegador y entra a [http://localhost:3000](http://localhost:3000/). Deberías ver tu aplicación hecha con React.

![https://lh4.googleusercontent.com/JM1O3LM0l0VlP6DzCv44Ml6HaNbvB-Ds2J0cnQR9s-3JzslZfldXWQ9Yywve9v2Xh9qO9IWaxqU05Fi9aCWG3wkMcmzDXdO2IU6gctehSFvd6TfgxD0xFSplzNoCFhJ5XOHVxkOv](https://lh4.googleusercontent.com/JM1O3LM0l0VlP6DzCv44Ml6HaNbvB-Ds2J0cnQR9s-3JzslZfldXWQ9Yywve9v2Xh9qO9IWaxqU05Fi9aCWG3wkMcmzDXdO2IU6gctehSFvd6TfgxD0xFSplzNoCFhJ5XOHVxkOv)

3. De hecho, si hiciste todo bien puedes cerrar VS Code y la aplicación seguirá funcionando sin problemas.

## Subir los cambios al repositorio de GitHub

1. Dentro del terminal ejecuta "_git add ._"

![https://lh6.googleusercontent.com/zbl9iBx4wsm4iTes2S8fzIEn6IkZKGOV1how1eGLcktS77Vo4wPeecKsZDpvxNfZM3WF9BPXfUxlKlrz7mPV1fLUrIeVoxsia6mTuEL3ugMNoLsLlpu0-jskbwOMZYXVBbcWVd6e](https://lh6.googleusercontent.com/zbl9iBx4wsm4iTes2S8fzIEn6IkZKGOV1how1eGLcktS77Vo4wPeecKsZDpvxNfZM3WF9BPXfUxlKlrz7mPV1fLUrIeVoxsia6mTuEL3ugMNoLsLlpu0-jskbwOMZYXVBbcWVd6e)

2. Luego ejecuta "_git status_" y verifica que se agrego el archivo "_Dockerfile_"

![https://lh3.googleusercontent.com/YpjmfLn-J9zsf_BOpMoDaJhknJrhfGBLUPOZwHg3SzNafakZR2UM243ZbxCt11FsNW7nD7ZSoe-IGixQ7UUi_FsM9QVPvWck2GfR5d35pgSnTgA3LrCmoYdkxwpV0JqDFge2oimB](https://lh3.googleusercontent.com/YpjmfLn-J9zsf_BOpMoDaJhknJrhfGBLUPOZwHg3SzNafakZR2UM243ZbxCt11FsNW7nD7ZSoe-IGixQ7UUi_FsM9QVPvWck2GfR5d35pgSnTgA3LrCmoYdkxwpV0JqDFge2oimB)

3. Luego ejecuta "_git commit -m "Add Dockerfile"_ "

![https://lh4.googleusercontent.com/PwRThi_YIprnnFIwg-zroLSuEl3zJrfllduDXbtfZ-rX5WV_c6uQGHwqN3s5XZPb9CEHAssazNbok_1nKLwoioiqx3o1j-5a3al5DIY65lb-MTy1ERcafa1W92Wl4rLjF7nITCkg](https://lh4.googleusercontent.com/PwRThi_YIprnnFIwg-zroLSuEl3zJrfllduDXbtfZ-rX5WV_c6uQGHwqN3s5XZPb9CEHAssazNbok_1nKLwoioiqx3o1j-5a3al5DIY65lb-MTy1ERcafa1W92Wl4rLjF7nITCkg)

4. Finalmente sube los cambios con "_git push_"

![https://lh6.googleusercontent.com/C4_vlWU_KeP_FQBuW1DY8G96YNQkJGDzXDFGmMPDWOChp7G3TjeengE7yb1PuKrKdjkIYIZdDCkOK4nSCDfn61BJn5w_xe3HjqEiYuJX52cVG9pD6SY8lhWdhQwIED01evIkgscK](https://lh6.googleusercontent.com/C4_vlWU_KeP_FQBuW1DY8G96YNQkJGDzXDFGmMPDWOChp7G3TjeengE7yb1PuKrKdjkIYIZdDCkOK4nSCDfn61BJn5w_xe3HjqEiYuJX52cVG9pD6SY8lhWdhQwIED01evIkgscK)

## Subir el contenedor de la aplicación a Docker Hub

1. Entra a [https://hub.docker.com/](https://hub.docker.com/).
2. Crea una cuenta o inicia sesión

![https://lh5.googleusercontent.com/OTKUpbBTdbAaRcmfi0wUbprf04Wx_6mHQp1IA1yhFY6R2XJEMTiQfprcopsYwz7m-MsaSFlQpzeSkKfK2jf85CUW92AGuOlJRom0MZ-GSOIMp1FLMeHPHius5m6womYZAhoZkAHW](https://lh5.googleusercontent.com/OTKUpbBTdbAaRcmfi0wUbprf04Wx_6mHQp1IA1yhFY6R2XJEMTiQfprcopsYwz7m-MsaSFlQpzeSkKfK2jf85CUW92AGuOlJRom0MZ-GSOIMp1FLMeHPHius5m6womYZAhoZkAHW)

3. Fíjate en el nombre de usuario que aparece arriba a la derecha. Lo vamos a usar más adelante.

![https://lh5.googleusercontent.com/gJd3GLmOfuZVgpSy5fUYi0Mk-1cSkKe7Om_iTvJoTqsf96ydyf98ixLARuXtby_q3uLkPV2h_fiIhZ_lRrzLY73xMC91vANL2L7rhMLH3dhxqkF0RZaf0JL2W6LGtvtDkgQC0CdT](https://lh5.googleusercontent.com/gJd3GLmOfuZVgpSy5fUYi0Mk-1cSkKe7Om_iTvJoTqsf96ydyf98ixLARuXtby_q3uLkPV2h_fiIhZ_lRrzLY73xMC91vANL2L7rhMLH3dhxqkF0RZaf0JL2W6LGtvtDkgQC0CdT)

4. Vuelve a la terminal del proyecto en Visual Studio. Dentro del terminal ejecuta "_docker login_". Este comando se utiliza para iniciar sesión desde el terminal.

![https://lh6.googleusercontent.com/0-9d48rAyi8_HvF1Q6QvjAv0JiJ7d7-v3DakNvDwy-bRNJ1ap-rODsZJ1pK-v8rUMJKi1bbY6ma42eND2YkHxDQCFmZZcYGKcc2ZefvoBL9nK0cK06SAUxvFQV_pQV-BQsxMUJcX](https://lh6.googleusercontent.com/0-9d48rAyi8_HvF1Q6QvjAv0JiJ7d7-v3DakNvDwy-bRNJ1ap-rODsZJ1pK-v8rUMJKi1bbY6ma42eND2YkHxDQCFmZZcYGKcc2ZefvoBL9nK0cK06SAUxvFQV_pQV-BQsxMUJcX)

**\*NOTA:** aquí deberás iniciar sesión con la cuenta que creaste anteriormente.\*

5. Crear un build de tu aplicación utilizando "_docker build -t **username**/my-app ._" (Reemplaza username por tu nombre de usuario)

![https://lh6.googleusercontent.com/cC9YjTzLoszvTj60C_krdbWyvEwwQaD5bhBXE2bWfeVttUhUdV-yxbL8oCbm0mf14x49aBQv53-jP7gqT7NU7_bJNlg2F5SvQIX-oBOHztEwAXg44eLs2Qv-SlgF36KyxIBEnWMM](https://lh6.googleusercontent.com/cC9YjTzLoszvTj60C_krdbWyvEwwQaD5bhBXE2bWfeVttUhUdV-yxbL8oCbm0mf14x49aBQv53-jP7gqT7NU7_bJNlg2F5SvQIX-oBOHztEwAXg44eLs2Qv-SlgF36KyxIBEnWMM)

6. Utiliza el comando "_docker push **username**/my-app_" para subir el contenedor de tu app a Docker Hub. (Reemplaza username por tu nombre de usuario)

![https://lh6.googleusercontent.com/d9KguAuCkCVIrlToX1WkEKKhijeA2TDm2mRBERDj6kglukT04xFwgi4-iOQ0uX48r8NSPGowIKyhbNKe7M9xDYeCIyWBfTtw0qQ71X5LPzH8sK6WcfXVA0NI1Hwwq90S7w_781_0](https://lh6.googleusercontent.com/d9KguAuCkCVIrlToX1WkEKKhijeA2TDm2mRBERDj6kglukT04xFwgi4-iOQ0uX48r8NSPGowIKyhbNKe7M9xDYeCIyWBfTtw0qQ71X5LPzH8sK6WcfXVA0NI1Hwwq90S7w_781_0)

7. Para verificar que hiciste todo bien ve a tu perfil de Docker Hub. Ahí debería aparecer el repositorio "**\*username**/my-app\*". Si hiciste los pasos bien no deberías tener problemas.

![https://lh3.googleusercontent.com/BCAvM1HQ2v0PFaowmIjUZljQXMDbFkZKLzT8-_HFZVHRB9F6MDBC9Qm-kWGuP2_KZAy70QD6Eu9JZ5G4VtWbXau2nPJrN49Dp7pIAtXwn246_G4jUsYD9uiDmxwK7vR-xSKsuQ-Q](https://lh3.googleusercontent.com/BCAvM1HQ2v0PFaowmIjUZljQXMDbFkZKLzT8-_HFZVHRB9F6MDBC9Qm-kWGuP2_KZAy70QD6Eu9JZ5G4VtWbXau2nPJrN49Dp7pIAtXwn246_G4jUsYD9uiDmxwK7vR-xSKsuQ-Q)

**REFERENCIAS:**

[https://docs.docker.com/get-started/overview/](https://docs.docker.com/get-started/overview/)

[https://mherman.org/blog/dockerizing-a-react-app/](https://mherman.org/blog/dockerizing-a-react-app/)

**Material adicional para seguir aprendiendo sobre Docker:**

- [https://docs.docker.com/](https://docs.docker.com/)
- [https://youtu.be/CV_Uf3Dq-EU](https://youtu.be/CV_Uf3Dq-EU)
- [https://youtu.be/NVvZNmfqg6M](https://youtu.be/NVvZNmfqg6M)
