<!DOCTYPE html>
<html lang="ko">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>파이썬 문자열 인덱스 시각화</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 20px;
        }

        .container {
            background: white;
            border-radius: 20px;
            box-shadow: 0 20px 60px rgba(0, 0, 0, 0.3);
            padding: 40px;
            max-width: 1200px;
            width: 100%;
        }

        h1 {
            color: #333;
            text-align: center;
            margin-bottom: 30px;
            font-size: 2.5em;
        }

        .input-section {
            margin-bottom: 40px;
            text-align: center;
        }

        label {
            display: block;
            font-size: 1.2em;
            color: #555;
            margin-bottom: 10px;
            font-weight: bold;
        }

        input[type="text"] {
            width: 100%;
            max-width: 600px;
            padding: 15px 20px;
            font-size: 1.2em;
            border: 3px solid #667eea;
            border-radius: 10px;
            outline: none;
            transition: border-color 0.3s;
        }

        input[type="text"]:focus {
            border-color: #764ba2;
        }

        .visualization {
            margin-top: 50px;
            padding: 30px;
            background: #f8f9fa;
            border-radius: 15px;
            overflow-x: auto;
        }

        .string-display {
            display: flex;
            justify-content: center;
            align-items: center;
            flex-wrap: wrap;
            gap: 5px;
            margin: 20px 0;
            min-height: 200px;
        }

        .char-container {
            display: flex;
            flex-direction: column;
            align-items: center;
            margin: 0 3px;
        }

        .index-forward {
            font-size: 0.9em;
            color: #667eea;
            font-weight: bold;
            margin-bottom: 5px;
            min-height: 25px;
            display: flex;
            align-items: center;
        }

        .char-box {
            width: 50px;
            height: 50px;
            background: #ffd700;
            border: 2px solid #ffa500;
            border-radius: 8px;
            display: flex;
            justify-content: center;
            align-items: center;
            font-size: 1.5em;
            font-weight: bold;
            color: #333;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.2);
            cursor: pointer;
            transition: all 0.2s;
            user-select: none;
        }

        .char-box:hover {
            transform: scale(1.05);
            box-shadow: 0 3px 8px rgba(0, 0, 0, 0.3);
        }

        .char-box.space {
            background: #e0e0e0;
            border-color: #b0b0b0;
        }

        .index-reverse {
            font-size: 0.9em;
            color: #764ba2;
            font-weight: bold;
            margin-top: 5px;
            min-height: 25px;
            display: flex;
            align-items: center;
        }

        .label-section {
            display: flex;
            justify-content: space-around;
            margin-bottom: 20px;
            font-size: 1.1em;
            font-weight: bold;
            color: #555;
        }

        .info-box {
            background: #e3f2fd;
            border-left: 4px solid #2196f3;
            padding: 15px;
            margin-top: 30px;
            border-radius: 5px;
        }

        .info-box h3 {
            color: #1976d2;
            margin-bottom: 10px;
        }

        .info-box p {
            color: #555;
            line-height: 1.6;
        }

        .info-box.slicing-info {
            background: #fff3cd;
            border-left: 4px solid #ffc107;
            margin-top: 20px;
        }

        .info-box.slicing-info h3 {
            color: #856404;
        }

        .empty-state {
            text-align: center;
            color: #999;
            font-size: 1.2em;
            padding: 50px;
        }

        .slicing-section {
            margin-top: 30px;
            padding: 25px;
            background: #fff3cd;
            border-radius: 15px;
            border: 2px solid #ffc107;
        }

        .slicing-section h2 {
            color: #856404;
            margin-bottom: 20px;
            font-size: 1.5em;
        }

        .slicing-input-group {
            display: flex;
            gap: 10px;
            align-items: center;
            flex-wrap: wrap;
            justify-content: center;
            margin-bottom: 20px;
        }

        .slicing-input-group input {
            max-width: 300px;
            font-family: 'Courier New', monospace;
            height: 54px;
            box-sizing: border-box;
        }

        .slicing-result {
            margin-top: 0;
            padding: 0;
            background: white;
            border-radius: 10px;
            border: 2px solid #ffc107;
            height: 54px;
            display: flex;
            align-items: center;
            box-sizing: border-box;
        }

        .slicing-result-text {
            font-family: 'Courier New', monospace;
            font-size: 1.3em;
            color: #333;
            padding: 10px 15px;
            background: #f8f9fa;
            border-radius: 5px;
            word-break: break-all;
            width: 100%;
            height: 100%;
            display: flex;
            align-items: center;
            box-sizing: border-box;
        }

        .char-box.selected {
            background: #4caf50;
            border-color: #2e7d32;
            transform: scale(1.1);
            z-index: 10;
            box-shadow: 0 4px 10px rgba(76, 175, 80, 0.5);
        }

        .char-box.selected.space {
            background: #81c784;
            border-color: #4caf50;
        }

        .error-message {
            color: #d32f2f;
            background: #ffebee;
            padding: 10px;
            border-radius: 5px;
            margin-top: 10px;
            border-left: 4px solid #d32f2f;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>🐍 파이썬 문자열 인덱싱 시각화</h1>
        
        <div class="input-section">
            <label for="stringInput">문자열을 입력하세요:</label>
            <input type="text" id="stringInput" placeholder="예: hello world" value="hello world">
        </div>

        <div class="slicing-section">
            <h2>🔪 슬라이싱 (Slicing)</h2>
            <div class="slicing-input-group">
                <input type="text" id="sliceInput" placeholder="예: [0:5], [::-1], [2:8:2]" value="">
                <span style="font-size: 1.5em;">✨</span>
                <div id="sliceResult" class="slicing-result" style="display: none;">
                    <div class="slicing-result-text" id="sliceResultText"></div>
                </div>
            </div>
            <div id="sliceError" class="error-message" style="display: none;"></div>
        </div>

        <div class="visualization" id="visualization">
            <div class="empty-state">위에 문자열을 입력하면 인덱싱이 시각적으로 표시됩니다.</div>
        </div>
    </div>

    <script>
        const stringInput = document.getElementById('stringInput');
        const sliceInput = document.getElementById('sliceInput');
        const visualization = document.getElementById('visualization');
        const sliceResult = document.getElementById('sliceResult');
        const sliceResultText = document.getElementById('sliceResultText');
        const sliceError = document.getElementById('sliceError');

        let currentString = '';
        let selectedIndices = new Set();
        let clickedIndices = new Set();
        let lastClickedIndex = null;

        // 선택된 인덱스들을 슬라이싱 문법으로 변환
        function indicesToSliceSyntax(indices, strLength) {
            if (indices.size === 0) return '';
            
            const sorted = Array.from(indices).sort((a, b) => a - b);
            
            // 연속된 범위인지 확인
            let isConsecutive = true;
            for (let i = 1; i < sorted.length; i++) {
                if (sorted[i] !== sorted[i-1] + 1) {
                    isConsecutive = false;
                    break;
                }
            }
            
            if (isConsecutive) {
                // 연속된 범위일 때 슬라이싱 문법 생성
                const start = sorted[0];
                const stop = sorted[sorted.length - 1] + 1;
                return `[${start}:${stop}]`;
            } else {
                // 연속되지 않은 경우, 선택된 범위를 표시
                // (실제로는 이 범위의 모든 문자가 선택되지는 않지만, 범위를 보여줌)
                const start = sorted[0];
                const stop = sorted[sorted.length - 1] + 1;
                return `[${start}:${stop}]`;
            }
        }

        // 슬라이싱 파싱 함수
        function parseSlice(sliceStr, strLength) {
            // 대괄호 제거
            sliceStr = sliceStr.trim();
            if (sliceStr.startsWith('[') && sliceStr.endsWith(']')) {
                sliceStr = sliceStr.slice(1, -1);
            }

            const parts = sliceStr.split(':');
            let start = null;
            let stop = null;
            let step = null;

            if (parts.length === 1) {
                // 단일 인덱스 [5]
                const idx = parseInt(parts[0]);
                if (isNaN(idx)) return null;
                return { indices: [idx], result: strLength > 0 && idx >= -strLength && idx < strLength ? [idx] : [] };
            }

            // start 파싱
            if (parts[0] !== '') {
                start = parseInt(parts[0]);
                if (isNaN(start)) return null;
                if (start < 0) start = strLength + start;
            } else {
                start = null;
            }

            // stop 파싱
            if (parts.length > 1 && parts[1] !== '') {
                stop = parseInt(parts[1]);
                if (isNaN(stop)) return null;
                if (stop < 0) stop = strLength + stop;
            } else {
                stop = null;
            }

            // step 파싱
            if (parts.length > 2 && parts[2] !== '') {
                step = parseInt(parts[2]);
                if (isNaN(step) || step === 0) return null;
            } else {
                step = 1;
            }

            // 인덱스 계산
            const indices = [];
            let current = start !== null ? start : (step > 0 ? 0 : strLength - 1);
            const end = stop !== null ? stop : (step > 0 ? strLength : -1);

            if (step > 0) {
                if (start === null) start = 0;
                if (stop === null) stop = strLength;
                for (let i = start; i < stop; i += step) {
                    if (i >= 0 && i < strLength) {
                        indices.push(i);
                    }
                }
            } else {
                if (start === null) start = strLength - 1;
                if (stop === null) stop = -1;
                for (let i = start; i > stop; i += step) {
                    if (i >= 0 && i < strLength) {
                        indices.push(i);
                    }
                }
            }

            return { indices, result: indices };
        }

        function visualizeString(str, sliceStr = '', useClickedIndices = false) {
            currentString = str;

            if (!str) {
                visualization.innerHTML = '<div class="empty-state">위에 문자열을 입력하면 인덱싱이 시각적으로 표시됩니다.</div>';
                sliceResult.style.display = 'none';
                sliceError.style.display = 'none';
                clickedIndices.clear();
                selectedIndices.clear();
                return;
            }

            // 클릭된 인덱스 사용
            if (useClickedIndices && clickedIndices.size > 0) {
                selectedIndices = new Set(clickedIndices);
                const sortedIndices = Array.from(clickedIndices).sort((a, b) => a - b);
                const resultStr = sortedIndices.map(i => str[i]).join('');
                sliceResultText.textContent = `"${resultStr}"`;
                sliceResult.style.display = 'block';
                sliceError.style.display = 'none';
                const sliceSyntax = indicesToSliceSyntax(clickedIndices, str.length);
                // 연속된 범위일 때만 슬라이싱 문법을 입력 필드에 표시
                if (sliceSyntax) {
                    sliceInput.value = sliceSyntax;
                }
                // 연속되지 않은 경우 입력 필드는 그대로 유지 (이전 값 또는 빈 값)
            }
            // 슬라이싱 처리
            else if (sliceStr) {
                const parsed = parseSlice(sliceStr, str.length);
                if (parsed) {
                    selectedIndices = new Set(parsed.indices);
                    clickedIndices = new Set(parsed.indices);
                    // 인덱스를 정렬하여 올바른 순서로 결과 문자열 생성
                    const sortedIndices = [...parsed.indices].sort((a, b) => a - b);
                    const resultStr = sortedIndices.map(i => str[i]).join('');
                    sliceResultText.textContent = `"${resultStr}"`;
                    sliceResult.style.display = 'block';
                    sliceError.style.display = 'none';
                } else {
                    sliceResult.style.display = 'none';
                    sliceError.textContent = '올바른 슬라이싱 문법을 입력하세요. 예: [0:5], [::-1], [2:8:2]';
                    sliceError.style.display = 'block';
                    selectedIndices.clear();
                }
            } else {
                sliceResult.style.display = 'none';
                sliceError.style.display = 'none';
                selectedIndices.clear();
            }

            const labelSection = document.createElement('div');
            labelSection.className = 'label-section';
            labelSection.innerHTML = '<div>인덱스(정방향)</div><div>인덱스(역방향)</div>';

            const stringDisplay = document.createElement('div');
            stringDisplay.className = 'string-display';

            for (let i = 0; i < str.length; i++) {
                const charContainer = document.createElement('div');
                charContainer.className = 'char-container';

                // 정방향 인덱스
                const indexForward = document.createElement('div');
                indexForward.className = 'index-forward';
                indexForward.textContent = i;
                charContainer.appendChild(indexForward);

                // 문자 박스
                const charBox = document.createElement('div');
                charBox.className = 'char-box';
                charBox.dataset.index = i;
                if (selectedIndices.has(i)) {
                    charBox.classList.add('selected');
                }
                if (str[i] === ' ') {
                    charBox.classList.add('space');
                    charBox.innerHTML = '&nbsp;';
                } else {
                    charBox.textContent = str[i];
                }
                
                // 클릭 이벤트 추가
                charBox.addEventListener('click', function(e) {
                    const index = parseInt(this.dataset.index);
                    
                    if (e.shiftKey && lastClickedIndex !== null) {
                        // Shift+클릭: 범위 선택
                        const start = Math.min(lastClickedIndex, index);
                        const end = Math.max(lastClickedIndex, index);
                        for (let j = start; j <= end; j++) {
                            clickedIndices.add(j);
                        }
                    } else {
                        // 일반 클릭: 토글
                        if (clickedIndices.has(index)) {
                            clickedIndices.delete(index);
                        } else {
                            clickedIndices.add(index);
                        }
                    }
                    
                    lastClickedIndex = index;
                    visualizeString(currentString, '', true);
                });
                
                charContainer.appendChild(charBox);

                // 역방향 인덱스
                const indexReverse = document.createElement('div');
                indexReverse.className = 'index-reverse';
                indexReverse.textContent = -(str.length - i);
                charContainer.appendChild(indexReverse);

                stringDisplay.appendChild(charContainer);
            }

            visualization.innerHTML = '';
            visualization.appendChild(labelSection);
            visualization.appendChild(stringDisplay);
        }

        // 초기 로드 시 시각화
        visualizeString(stringInput.value, sliceInput.value);

        // 문자열 입력 시 실시간 업데이트
        stringInput.addEventListener('input', function() {
            clickedIndices.clear();
            lastClickedIndex = null;
            visualizeString(this.value, sliceInput.value);
        });

        // 슬라이싱 입력 시 실시간 업데이트
        sliceInput.addEventListener('input', function() {
            clickedIndices.clear();
            lastClickedIndex = null;
            visualizeString(stringInput.value, this.value);
        });
    </script>
</body>
</html>
