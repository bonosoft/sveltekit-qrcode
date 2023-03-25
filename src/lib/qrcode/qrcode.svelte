<script lang="ts">
import { QRCode } from "./qrcode";
import type { Options } from "./qrcode";

export let content = '';

export let size = '150';
export let padding = '4';
export let color = '#000000';
export let bgcolor = '#ffffff';
export let responsive = 'false';
export let errorCorrection = 'M';

let opt : Options = { content: content,
    padding: parseInt(padding), width: parseInt(size), height: parseInt(size), typeNumber: 4, color: color, 
    background: bgcolor, ecl: errorCorrection, container: responsive.toLowerCase() == 'true'?'svg-viewbox':'svg',
    join: true };

let qrCode = new QRCode(opt);

</script>

{@html qrCode.svg()}
